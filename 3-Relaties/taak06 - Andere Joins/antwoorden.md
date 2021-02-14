# Antwoorden

1. Copy paste je gemaakte SQL query hieronder
   SELECT name, platform FROM game LEFT JOIN platform ON game.platform_id = platform.id WHERE name LIKE 'Grand Theft Auto%'
2. Copy paste je gemaakte SQL query hieronder
   SELECT platform, name FROM game RIGHT JOIN platform ON game.platform_id = platform.id WHERE platform.platform = 'SCD'
