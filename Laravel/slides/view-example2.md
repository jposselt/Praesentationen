# View Beispiel


```html
<!-- Stored in resources/views/pages/users.blade.php -->

@extends('layouts.app')

@section('title', 'User List')

@section('content')
<table>
	<tr>
    	<th>Firstname</th>
    	<th>Lastname</th> 
	</tr>
	@foreach($users as $user)
	<tr>
	    <td>{{$user->first_name}}</td> <!-- <?php echo htmlspecialchars($user->first_name); ?> -->
	    <td>{{$user->last_name}}</td> <!-- Schützt vor Cross-site Scripting (XSS) ?> -->
	</tr>
	@endforeach
</table>
@endsection
```