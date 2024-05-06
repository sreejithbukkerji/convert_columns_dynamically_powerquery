# convert_columns_dynamically_powerquery
Transform and convert multiple columns into a different data type 
I have a table with more than a dozen date columns and many text columns. I have a business requirement to combine all those columns into a single string. 
Before combining, the dates which are currently in the mm/dd/yyyy to be converted to dd.mm.yyyy format. Since going through each of these columns and converting them is a tedious task, this should be done dynamically.
Luckily, we have options to do this in Power Query.
My solution is to use Table.Schema, List.Transform and Table.TransformColumns to achieve the desired outcome.
