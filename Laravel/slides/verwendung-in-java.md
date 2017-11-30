#Verwendung in Java

```
import java.io.BufferedReader;
import java.io.InputStreamReader;
import java.net.HttpURLConnection;
import java.net.URL;
public class TestServerRequest {
    public static void main(String[] args) {
        int id = 1;
        try {
            URL url = new URL("https://restapi.url/api/data/" + id);
            HttpURLConnection conn = (HttpURLConnection) url.openConnection();
            conn.setRequestMethod("GET");
            System.out.println(conn.getResponseCode());
            BufferedReader reader = new BufferedReader(new InputStreamReader(conn.getInputStream()));
            String output;
            while ((output = reader.readLine()) != null) {
                System.out.println(output);
            }
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
```