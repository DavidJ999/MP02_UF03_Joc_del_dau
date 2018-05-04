# Agafo o no

Aquesta funció és queda tots aquells numeros que siguin més grans que 2.

```
create function dbo.quedo (@numjugador as int,@punts as int)
returns integer
as begin
	declare @sino int;
	if @punts between 0 and 2
		begin
			set @sino=0
		end;
	else 
		begin
			set @sino=1
		end;
	return @sino
end;
```
