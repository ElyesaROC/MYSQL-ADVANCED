# Antwoorden

1. Copy paste je gemaakte SQL query hieronder
   SELECT * FROM `game` LEFT JOIN platform ON game.platform_id = platform.id
2. Copy paste je gemaakte SQL query hieronder
   SELECT * FROM `game` ORDER BY id LIMIT 10
3. Copy paste je gemaakte SQL query hieronder
   SELECT name,platform FROM `game` LEFT JOIN platform ON game.platform_id = platform.id  WHERE name = 'Call of Duty: Advanced Warfare'
4. Copy paste je gemaakte SQL query hieronder
   SELECT platform, name FROM `game` LEFT JOIN platform ON game.platform_id = platform.id  WHERE name LIKE 'FIFA%'
5. Copy paste je gemaakte SQL query hieronder
SELECT name, platform FROM `game` LEFT JOIN platform ON game.platform_id = platform.id  WHERE name = 'Borderlands' OR name = 'Borderlands 2'