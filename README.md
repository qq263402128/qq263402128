- 👋 Hi, I’m @qq263402128
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- :x:
- :snake:
- :recycle:
- :arrow_up:
- :arrow_down:

<!---
qq263402128/qq263402128 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

`sql
SELECT
	a.id,
	a.`name`,
	( SELECT GROUP_CONCAT( `name` ) FROM game_type WHERE FIND_IN_SET( id, a.tid ) > 0 ) AS types 
FROM
	game a,
	game_type b 
WHERE
	a.tid = b.id
`
