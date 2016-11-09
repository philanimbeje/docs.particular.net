The SQL Server transport runs a periodic task that removes expired messages from the queue. The task is first executed when the endpoint starts and is subsequently scheduled to execute 5 minutes after the previous run of the task has been completed. Expired messages are not received from the queue and their disk space will be reclaimed when the periodic task executes.