### Дата рождения.

```postgresql
ALTER TABLE Person ADD COLUMN date_of_birth DATE;
```

```java
@Column(name = "date_of_birth")
@Temporal(TemporalType.DATE)
@DateTimeFormat(pattern = "dd/MM/yyyy") // дд/мм/гггг
private Date dateOfBirth;
```

### Точное время создания.

```postgresql
ALTER TABLE Person ADD COLUMN created_at TIMESTAMP;
```

```java
@Column(name = "created_at")
@Temporal(TemporalType.TIMESTAMP)
private Date createdAt;
```