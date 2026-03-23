SELECT TEAM, SHIRT_OR_HAT, FIRST_NAME, LAST_NAME
FROM participants
WHERE STATE = 'CO'
ORDER BY TEAM ASC, SHIRT_OR_HAT ASC, LAST_NAME DESC;


SELECT 
    states.state_name AS STATE_NAME, 
    MAX(people.quiz_points) AS MAXPOINTS, 
    AVG(people.quiz_points) AS AVGPOINTS
FROM states
JOIN people ON states.state_abbrev = people.state_code
GROUP BY states.state_name
ORDER BY AVGPOINTS DESC;
