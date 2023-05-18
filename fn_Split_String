create function dbo.fn_Split_String
(
	@String nvarchar(max),
	@Delimiter nchar(1)
)
returns @output table(Id bigint identity(1,1), Data nvarchar(max)) 
begin 
		declare @start int, @end int

		select @start = 1, @end = charindex(@delimiter, @string) 

		while @start < len(@string) + 1 
		begin 
				if @end = 0  
					SET @end = len(@string) + 1
       
				insert into @output (Data)  
				values(substring(@string, @start, @end - @start)) 

				SET @start = @end + 1 
				SET @end = charindex(@delimiter, @string, @start)
		end 

		return 
end
