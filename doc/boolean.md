# Oracle Database 23c

## Boolean Data Type

You can definie a boolean data type using the `BOOLEAN` or `BOOL` keywords.

	create table boolean_tab (
		id		number		generated always as identity,
		active	boolean		
	);

You can assign a value to boolean data type in a number of ways. Here some examples.

	insert into boolean_tab vales (active) values (true);
	insert into boolean_tab vales (active) values ('true');
	insert into boolean_tab vales (active) values ('yes');
	insert into boolean_tab vales (active) values (1);

	insert into boolean_tab vales (active) values (false);
	insert into boolean_tab vales (active) values ('false');
	insert into boolean_tab vales (active) values ('no');
	insert into boolean_tab vales (active) values (0);

	commit;

You can use boolean data type in SQL expression.

	select count(*)
	  from boolean_tab
	 where active;

	COUNT(*)
	--------
	       4





