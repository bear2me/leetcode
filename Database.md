<https://leetcode.com/problemset/database/>

// Sorted By Acceptence

[595. Big Countries](https://leetcode.com/problems/big-countries/)

```sql
select name, population, area from World where area > 3000000 or population > 25000000
```

[627. Swap Salary](https://leetcode.com/problems/swap-salary/)

```sql
-- solution1
update salary set sex=IF(sex='m','f','m')
-- solution2
update salary 
set sex = case
	when sex = 'f' then 'm'
	when sex = 'm' then 'f'
end
```

IF的用法

CASE WHEN

[620. Not Boring Movies](https://leetcode.com/problems/not-boring-movies/description/)

```sql
select * from cinema where id%2=1 and description!='boring' order by rating desc
```

id%2 取余