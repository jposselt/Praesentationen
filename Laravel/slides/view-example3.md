# View Beispiel

```html
<html>
    <head>
        <title>App Name - User List</title>
    </head>
    <body>
        <div class="container">
            <table>
				<tr>
    				<th>Firstname</th>
    				<th>Lastname</th> 
				</tr>
				<?php foreach($users as $user){ ?>
				<tr>
	    			<td><?php echo htmlspecialchars($user->first_name); ?></td>
	    			<td><?php echo htmlspecialchars($user->last_name); ?></td> 
				</tr>
				<?php } ?>
			</table>
        </div>
    </body>
</html>
```