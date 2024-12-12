#### Дата рождения.
```java
@Column(name = "date_of_birth")
@Temporal(TemporalType.DATE)
@DateTimeFormat(pattern = "dd/MM/yyyy") // дд/мм/гггг
private Date dateOfBirth;
```
#### Точное время создания.
```java
@Column(name = "created_at")
@Temporal(TemporalType.TIMESTAMP)
private Date createdAt;
```