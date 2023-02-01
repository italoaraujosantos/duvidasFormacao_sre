Todos as requisições efetuadas a base de dados são recusadas, a princio achei que estava 
relacionado ao tempo de repetição das requisições efetuadas pelo proxy.

Mas o que eu não conseguir identificar foi o motivo do sgbd mysql não subir mesmo com mais de um minuto de execução da stack.


# HELP http_server_requests_seconds  
# TYPE http_server_requests_seconds histogram
http_server_requests_seconds_bucket{application="app-forum-api",exception="CannotCreateTransactionException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos/{id}",le="0.05",} 0.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="CannotCreateTransactionException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos/{id}",le="0.1",} 0.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="CannotCreateTransactionException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos/{id}",le="0.2",} 0.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="CannotCreateTransactionException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos/{id}",le="0.3",} 0.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="CannotCreateTransactionException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos/{id}",le="0.5",} 0.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="CannotCreateTransactionException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos/{id}",le="1.0",} 0.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="CannotCreateTransactionException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos/{id}",le="+Inf",} 41.0
http_server_requests_seconds_count{application="app-forum-api",exception="CannotCreateTransactionException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos/{id}",} 41.0
http_server_requests_seconds_sum{application="app-forum-api",exception="CannotCreateTransactionException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos/{id}",} 41.927510049
http_server_requests_seconds_bucket{application="app-forum-api",exception="RedisConnectionFailureException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos",le="0.05",} 78.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="RedisConnectionFailureException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos",le="0.1",} 78.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="RedisConnectionFailureException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos",le="0.2",} 78.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="RedisConnectionFailureException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos",le="0.3",} 78.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="RedisConnectionFailureException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos",le="0.5",} 78.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="RedisConnectionFailureException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos",le="1.0",} 78.0
http_server_requests_seconds_bucket{application="app-forum-api",exception="RedisConnectionFailureException",method="GET",outcome="SERVER_ERROR",status="500",uri="/topicos",le="+Inf",} 79.0

