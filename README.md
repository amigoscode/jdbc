# Working with Databases in Java
- JDBC
- Datasource
- Connection Pool
- Flyway and JDBC Template

# Diagram
![diagram](https://user-images.githubusercontent.com/40702606/132997719-73170303-30a6-499b-9c59-4143ba0f8439.png)

# How to get started
- switch to branch `git checkout start`
- watch YouTube video

# Exercise
- Add the ability to edit movies
- Add `actor` table and associate them with movies
You will need to create a new migration called: `V1__ActorTable.sql` and the following sql to create the actor table
```sql
CREATE TABLE actor
(
    id    bigserial primary key,
    name  TEXT NOT NULL,
    movie bigint REFERENCES movie (id),
    unique (name, movie)
);
```

# Join the community
<p>
    <a href="https://discord.com/invite/S7gXXxq8" alt="Contributors">
        <img src="https://img.shields.io/discord/699965319883784252" />
    </a>
</p>
