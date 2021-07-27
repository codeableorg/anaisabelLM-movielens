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
SELECT title, release_date FROM movies WHERE release_date = '1995-01-01';

                                title                                | release_date 
---------------------------------------------------------------------+--------------
 Toy Story (1995)                                                    | 1995-01-01
 GoldenEye (1995)                                                    | 1995-01-01
 Four Rooms (1995)                                                   | 1995-01-01
 Get Shorty (1995)                                                   | 1995-01-01
 Copycat (1995)                                                      | 1995-01-01
 Shanghai Triad (Yao a yao yao dao waipo qiao) (1995)                | 1995-01-01
 Twelve Monkeys (1995)                                               | 1995-01-01
 Babe (1995)                                                         | 1995-01-01
 Dead Man Walking (1995)                                             | 1995-01-01
 Seven (Se7en) (1995)                                                | 1995-01-01
 French Twist (Gazon maudit) (1995)                                  | 1995-01-01
 White Balloon, The (1995)                                           | 1995-01-01
 Antonia's Line (1995)                                               | 1995-01-01
 Angels and Insects (1995)                                           | 1995-01-01
 Brothers McMullen, The (1995)                                       | 1995-01-01
 Bad Boys (1995)                                                     | 1995-01-01
 Apollo 13 (1995)                                                    | 1995-01-01
 Batman Forever (1995)                                               | 1995-01-01
 Crimson Tide (1995)                                                 | 1995-01-01
 Desperado (1995)                                                    | 1995-01-01
 Doom Generation, The (1995)                                         | 1995-01-01
 Free Willy 2: The Adventure Home (1995)                             | 1995-01-01
 Mad Love (1995)                                                     | 1995-01-01
 Net, The (1995)                                                     | 1995-01-01
 Strange Days (1995)                                                 | 1995-01-01
 To Wong Foo, Thanks for Everything! Julie Newmar (1995)             | 1995-01-01
 Billy Madison (1995)                                                | 1995-01-01
 Outbreak (1995)                                                     | 1995-01-01
 While You Were Sleeping (1995)                                      | 1995-01-01
 Operation Dumbo Drop (1995)                                         | 1995-01-01
 Heat (1995)                                                         | 1995-01-01
 Sabrina (1995)                                                      | 1995-01-01
 Sense and Sensibility (1995)                                        | 1995-01-01
 Leaving Las Vegas (1995)                                            | 1995-01-01
 Restoration (1995)                                                  | 1995-01-01
 Once Upon a Time... When We Were Colored (1995)                     | 1995-01-01
 Sudden Death (1995)                                                 | 1995-01-01
 Ace Ventura: When Nature Calls (1995)                               | 1995-01-01
 Powder (1995)                                                       | 1995-01-01
 Dangerous Minds (1995)                                              | 1995-01-01
--More-- 
```

3. List the `title` and `release_date` of all the movies released between `1996-01-01` and `1998-01-01`.

```SQL
SELECT title, release_date FROM movies WHERE release_date BETWEEN '1996-01-01' AND '1998-01-01';

                                      title                                      | release_date 
---------------------------------------------------------------------------------+--------------
 Richard III (1995)                                                              | 1996-01-22
 Mr. Holland's Opus (1995)                                                       | 1996-01-29
 From Dusk Till Dawn (1996)                                                      | 1996-02-05
 Muppet Treasure Island (1996)                                                   | 1996-02-16
 Braveheart (1995)                                                               | 1996-02-16
 Taxi Driver (1976)                                                              | 1996-02-16
 Rumble in the Bronx (1995)                                                      | 1996-02-23
 Birdcage, The (1996)                                                            | 1996-03-08
 Welcome to the Dollhouse (1995)                                                 | 1996-05-24
 Fargo (1996)                                                                    | 1997-02-14
 All Dogs Go to Heaven 2 (1996)                                                  | 1996-03-29
 Theodore Rex (1995)                                                             | 1996-03-29
 Sgt. Bilko (1996)                                                               | 1996-03-29
 Diabolique (1996)                                                               | 1996-01-01
 Moll Flanders (1996)                                                            | 1996-06-14
 Kids in the Hall: Brain Candy (1996)                                            | 1996-04-12
 Mystery Science Theater 3000: The Movie (1996)                                  | 1996-04-19
 Truth About Cats & Dogs, The (1996)                                             | 1996-04-26
 Flipper (1996)                                                                  | 1996-05-10
 Horseman on the Roof, The (Hussard sur le toit, Le) (1995)                      | 1996-04-19
 Wallace & Gromit: The Best of Aardman Animation (1996)                          | 1996-04-05
 Haunted World of Edward D. Wood Jr., The (1995)                                 | 1996-04-26
 Cold Comfort Farm (1995)                                                        | 1996-04-23
 Rock, The (1996)                                                                | 1996-06-07
 Twister (1996)                                                                  | 1996-05-10
 Striptease (1996)                                                               | 1996-06-28
 Independence Day (ID4) (1996)                                                   | 1996-07-03
 Cable Guy, The (1996)                                                           | 1996-06-14
 Frighteners, The (1996)                                                         | 1996-07-19
 Lone Star (1996)                                                                | 1996-06-21
 Phenomenon (1996)                                                               | 1996-06-29
 Spitfire Grill, The (1996)                                                      | 1996-09-06
 Supercop (1992)                                                                 | 1996-07-26
 Bound (1996)                                                                    | 1996-10-04
 Kansas City (1996)                                                              | 1996-08-16
 Big Night (1996)                                                                | 1996-09-20
 D3: The Mighty Ducks (1996)                                                     | 1996-10-04
 Unhook the Stars (1996)                                                         | 1996-10-30
 Long Kiss Goodnight, The (1996)                                                 | 1996-10-05
 Ghost and the Darkness, The (1996)                                              | 1996-10-11
 Jude (1996)                                                                     | 1996-11-01
 Swingers (1996)                                                                 | 1996-10-18
 Return of the Jedi (1983)                                                       | 1997-03-14
 Mirror Has Two Faces, The (1996)                                                | 1996-11-15
 Breaking the Waves (1996)                                                       | 1996-11-15
 Star Trek: First Contact (1996)                                                 | 1996-11-22
--More-- 
```

4. List the `title` of all movies that begins with the letter 'F'.

```SQL
SELECT title FROM movies WHERE title LIKE 'F%';

                          title                           
----------------------------------------------------------
 Four Rooms (1995)
 French Twist (Gazon maudit) (1995)
 From Dusk Till Dawn (1996)
 Free Willy 2: The Adventure Home (1995)
 Forrest Gump (1994)
 Four Weddings and a Funeral (1994)
 Faster Pussycat! Kill! Kill! (1965)
 Firm, The (1993)
 Free Willy (1993)
 Fugitive, The (1993)
 Fargo (1996)
 Flipper (1996)
 Frighteners, The (1996)
 Fish Called Wanda, A (1988)
 Full Metal Jacket (1987)
 Field of Dreams (1989)
 Fifth Element, The (1997)
 Full Monty, The (1997)
 Fierce Creatures (1997)
 Face/Off (1997)
 Fly Away Home (1996)
 FairyTale: A True Story (1997)
 Fallen (1998)
 Flintstones, The (1994)
 Fear of a Black Hat (1993)
 Fantasia (1940)
 Forbidden Planet (1956)
 Free Willy 3: The Rescue (1997)
 First Wives Club, The (1996)
 Fly Away Home (1996)
 Farinelli: il castrato (1994)
 Fatal Instinct (1993)
 Fan, The (1996)
 For Whom the Bell Tolls (1943)
 Father of the Bride (1950)
 Fog, The (1980)
 Fried Green Tomatoes (1991)
 Fire on the Mountain (1996)
 First Knight (1995)
 Fluke (1995)
 Father of the Bride Part II (1995)
 Fair Game (1995)
 French Kiss (1995)
 Frisk (1995)
 Faces (1968)
--More-- 
```

5. List the `title` of the oldest movie.

```SQL
SELECT title FROM movies ORDER BY release_date asc LIMIT 1;

                          title                           
----------------------------------------------------------
 Nosferatu (Nosferatu, eine Symphonie des Grauens) (1922)
(1 row)
```

6. List the `title` and `release_date` of all the movies from the newest to the oldest one.

```SQL
SELECT title, release_date  FROM movies ORDER BY release_date desc;

                                       title                                       | release_date 
-----------------------------------------------------------------------------------+--------------
 unknown                                                                           | 
 Apt Pupil (1998)                                                                  | 1998-10-23
 Mighty, The (1998)                                                                | 1998-10-09
 City of Angels (1998)                                                             | 1998-04-03
 Big One, The (1997)                                                               | 1998-03-27
 Spanish Prisoner, The (1997)                                                      | 1998-03-27
 Lost in Space (1998)                                                              | 1998-03-27
 Mercury Rising (1998)                                                             | 1998-03-27
 Niagara, Niagara (1997)                                                           | 1998-03-20
 Hana-bi (1997)                                                                    | 1998-03-20
 Object of My Affection, The (1998)                                                | 1998-03-20
 Primary Colors (1998)                                                             | 1998-03-20
 Price Above Rubies, A (1998)                                                      | 1998-03-20
 Man in the Iron Mask, The (1998)                                                  | 1998-03-17
 Newton Boys, The (1998)                                                           | 1998-03-14
 Wild Things (1998)                                                                | 1998-03-14
 Everest (1998)                                                                    | 1998-03-10
 U.S. Marshalls (1998)                                                             | 1998-03-10
 Love and Death on Long Island (1997)                                              | 1998-03-10
 Hush (1998)                                                                       | 1998-03-10
 Men With Guns (1997)                                                              | 1998-03-06
 Further Gesture, A (1996)                                                         | 1998-02-20
 Little City (1998)                                                                | 1998-02-20
 Palmetto (1998)                                                                   | 1998-02-20
 Wedding Singer, The (1998)                                                        | 1998-02-13
 Sphere (1998)                                                                     | 1998-02-13
 Ayn Rand: A Sense of Life (1997)                                                  | 1998-02-13
 Tokyo Fist (1995)                                                                 | 1998-02-11
 Replacement Killers, The (1998)                                                   | 1998-02-06
 Blues Brothers 2000 (1998)                                                        | 1998-02-06
 Mat' i syn (1997)                                                                 | 1998-02-06
 Night Flier (1997)                                                                | 1998-02-06
 B. Monkey (1998)                                                                  | 1998-02-06
 Nil By Mouth (1997)                                                               | 1998-02-06
 Tainted (1998)                                                                    | 1998-02-01
 Letter From Death Row, A (1998)                                                   | 1998-02-01
 Desperate Measures (1998)                                                         | 1998-01-30
 Deep Rising (1998)                                                                | 1998-01-30
 Desperate Measures (1998)                                                         | 1998-01-30
 Magic Hour, The (1998)                                                            | 1998-01-30
 Twilight (1998)                                                                   | 1998-01-30
 Four Days in September (1997)                                                     | 1998-01-23
 Dangerous Beauty (1998)                                                           | 1998-01-23
 Duoluo tianshi (1995)                                                             | 1998-01-21
 Prophecy II, The (1998)                                                           | 1998-01-16
 Hard Rain (1998)                                                                  | 1998-01-16
--More-- 
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
