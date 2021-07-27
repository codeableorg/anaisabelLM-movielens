# MovieLens Part 1

Copy and paste you SQL query replacing the lines `<your SQL query here>` inside each question.

0. List all the columns of the `genres` table.

```SQL
SELECT * FROM genres;
```
id |    name     
----+-------------
  1 | Action
  2 | Adventure
  3 | Animation
  4 | Children's
  5 | Comedy
  6 | Crime
  7 | Documentary
  8 | Drama
  9 | Fantasy
 10 | Film-Noir
 11 | Horror
 12 | Musical
 13 | Mystery
 14 | Romance
 15 | Sci-Fi
 16 | Thriller
 17 | War
 18 | Western
(18 rows)

1. List all the columns of the `movies` table.

```SQL
SELECT * FROM movies;

id  |                                       title                                       | release_date 
------+-----------------------------------------------------------------------------------+--------------
    1 | Toy Story (1995)                                                                  | 1995-01-01
    2 | GoldenEye (1995)                                                                  | 1995-01-01
    3 | Four Rooms (1995)                                                                 | 1995-01-01
    4 | Get Shorty (1995)                                                                 | 1995-01-01
    5 | Copycat (1995)                                                                    | 1995-01-01
    6 | Shanghai Triad (Yao a yao yao dao waipo qiao) (1995)                              | 1995-01-01
    7 | Twelve Monkeys (1995)                                                             | 1995-01-01
    8 | Babe (1995)                                                                       | 1995-01-01
    9 | Dead Man Walking (1995)                                                           | 1995-01-01
   10 | Richard III (1995)                                                                | 1996-01-22
   11 | Seven (Se7en) (1995)                                                              | 1995-01-01
   12 | Usual Suspects, The (1995)                                                        | 1995-08-14
   13 | Mighty Aphrodite (1995)                                                           | 1995-10-30
   14 | Postino, Il (1994)                                                                | 1994-01-01
   15 | Mr. Holland's Opus (1995)                                                         | 1996-01-29
   16 | French Twist (Gazon maudit) (1995)                                                | 1995-01-01
   17 | From Dusk Till Dawn (1996)                                                        | 1996-02-05
   18 | White Balloon, The (1995)                                                         | 1995-01-01
   19 | Antonia's Line (1995)                                                             | 1995-01-01
   20 | Angels and Insects (1995)                                                         | 1995-01-01
   21 | Muppet Treasure Island (1996)                                                     | 1996-02-16
   22 | Braveheart (1995)                                                                 | 1996-02-16
   23 | Taxi Driver (1976)                                                                | 1996-02-16
   24 | Rumble in the Bronx (1995)                                                        | 1996-02-23
   25 | Birdcage, The (1996)                                                              | 1996-03-08
   26 | Brothers McMullen, The (1995)                                                     | 1995-01-01
   27 | Bad Boys (1995)                                                                   | 1995-01-01
   28 | Apollo 13 (1995)                                                                  | 1995-01-01
   29 | Batman Forever (1995)                                                             | 1995-01-01
   30 | Belle de jour (1967)                                                              | 1967-01-01
   31 | Crimson Tide (1995)                                                               | 1995-01-01
   32 | Crumb (1994)                                                                      | 1994-01-01
   33 | Desperado (1995)                                                                  | 1995-01-01
   34 | Doom Generation, The (1995)                                                       | 1995-01-01
   35 | Free Willy 2: The Adventure Home (1995)                                           | 1995-01-01
   36 | Mad Love (1995)                                                                   | 1995-01-01
   37 | Nadja (1994)                                                                      | 1994-01-01
   38 | Net, The (1995)                                                                   | 1995-01-01
   39 | Strange Days (1995)                                                               | 1995-01-01
   40 | To Wong Foo, Thanks for Everything! Julie Newmar (1995)                           | 1995-01-01
   41 | Billy Madison (1995)                                                              | 1995-01-01
   42 | Clerks (1994)                                                                     | 1994-01-01
   43 | Disclosure (1994)                                                                 | 1994-01-01
   44 | Dolores Claiborne (1994)                                                          | 1994-01-01
   45 | Eat Drink Man Woman (1994)                                                        | 1994-01-01
   46 | Exotica (1994)                                                                    | 1994-01-01
   47 | Ed Wood (1994)                                                                    | 1994-01-01
--More-- 
```

2. List the `title` and `release_date` of all the movies released in `1995-01-01`.

```SQL
<your SQL query here>
```

3. List the `title` and `release_date` of all the movies released between `1996-01-01` and `1998-01-01`.

```SQL
<your SQL query here>
```

4. List the `title` of all movies that begins with the letter 'F'.

```SQL
<your SQL query here>
```

5. List the `title` of the oldest movie.

```SQL
<your SQL query here>
```

6. List the `title` and `release_date` of all the movies from the newest to the oldest one.

```SQL
<your SQL query here>
```

7. List all the years of release in ascending order without having repeated values.

```SQL
<your SQL query here>
```

8. List how many male and female users there are.

```SQL
<your SQL query here>
```

9. List how many users of each age there are.

```SQL
<your SQL query here>
```

10. List average age of the users group by gender.

```SQL
<your SQL query here>
```
