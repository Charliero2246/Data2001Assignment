# Data2001Assignment


# How to run

1. Install all modules required as shown in first codeblock, 
2. Make sure to run it using the .venv kernel by selecting it in vscode
3. Run each chunk of code top to bottom
4. Should the db connection freeze, open pgadmin and run
SELECT 
    pg_terminate_backend(pid)
FROM pg_stat_activity
WHERE datname = current_database()
  AND pid <> pg_backend_pid();
  then run each code block top to bottom again
  