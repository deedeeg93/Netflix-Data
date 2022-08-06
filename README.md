# Netflix-Data

--SELECT titles.title, titles.type, people.show_id, people.director
--FROM "CharlotteChaze/BreakIntoTech"."netflix_titles_info" titles
--LEFT JOIN "CharlotteChaze/BreakIntoTech"."netflix_people" people
--ON titles.show_id = people.show_id;

--SELECT count (*)
--FROM "CharlotteChaze/BreakIntoTech"."netflix_titles_info"
--WHERE type ='Movie';

--SELECT max(date(date_added))
--FROM "CharlotteChaze/BreakIntoTech"."netflix_titles_info"

--SELECT title
--FROM "CharlotteChaze/BreakIntoTech"."netflix_titles_info"
--ORDER BY title asc;

--SELECT director
--FROM "CharlotteChaze/BreakIntoTech". "netflix_people" people
--LEFT JOIN "CharlotteChaze/BreakIntoTech"."netflix_titles_info" titles
--ON people.show_id=titles.show_id
--WHERE titles.title= 'Bright Star';

SELECT title, release_year
FROM "CharlotteChaze/BreakIntoTech"."netflix_titles_info"
WHERE type ='Movie'
ORDER BY release_year asc
LIMIT 1;
