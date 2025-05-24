## formula

### get feed from repo-url

```
IF(ISNUMBER(SEARCH("release", [subscribe])), CONCATENATE([url], "/releases.atom"), IF(ISNUMBER(SEARCH("commit", [subscribe])), CONCATENATE([url], "/commits.atom"), ""))
```

## query

### order by multi-column

```
SELECT *
FROM `table_1`
ORDER BY `column_1` ASC, `column_2` ASC, `column_2` ASC;
```

### search in multi-column

```
SELECT *
FROM `table_1`
WHERE `column_1` LIKE '%string%'
OR `column_2` LIKE '%string%'
OR `column_3` LIKE '%string%';
```