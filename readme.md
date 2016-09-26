laravel REST api using:
jwt-auth,
dingo api,
laravel cors,
zizaco entrust.


| Host | Method    | URI                        | Name             | Action                                                                                                                        | Protected | Version(s) | Scope(s) | Rate Limit |
+------+-----------+----------------------------+------------------+-------------------------------------------------------------------------------------------------------------------------------+-----------+------------+----------+------------+
|      | POST      | /api/auth/login            |                  | App\Api\V1\Controllers\AuthController@login                                                                                   | No        | v1         |          |            |
|      | POST      | /api/auth/signup           |                  | App\Api\V1\Controllers\AuthController@signup                                                                                  | No        | v1         |          |            |
|      | POST      | /api/auth/recovery         |                  | App\Api\V1\Controllers\AuthController@recovery                                                                                | No        | v1         |          |            |
|      | POST      | /api/auth/reset            |                  | App\Api\V1\Controllers\AuthController@reset                                                                                   | No        | v1         |          |            |
|      | GET|HEAD  | /api/protected             |                  | [{"id":2,"name":"allen","email":"andycc77e@gmail.com","created_at":"2016-09-25 07:25:33","updated_at":"2016-09-25 07:25:33"}] | Yes       | v1         |          |            |
|      | GET|HEAD  | /api/free                  |                  | [{"id":2,"name":"allen","email":"andycc77e@gmail.com","created_at":"2016-09-25 07:25:33","updated_at":"2016-09-25 07:25:33"}] | No        | v1         |          |            |
|      | POST      | /api/auth/createRole       |                  | App\Api\V1\Controllers\AuthController@createRole                                                                              | No        | v1         |          |            |
|      | POST      | /api/auth/createPermission |                  | App\Api\V1\Controllers\AuthController@createPermission                                                                        | No        | v1         |          |            |
|      | POST      | /api/auth/assignRole       |                  | App\Api\V1\Controllers\AuthController@assignRole                                                                              | No        | v1         |          |            |
|      | POST      | /api/auth/attachPermission |                  | App\Api\V1\Controllers\AuthController@attachPermission                                                                        | No        | v1         |          |            |
|      | GET|HEAD  | /api/todo                  | api.todo.index   | App\Api\V1\Controllers\TodoController@index                                                                                   | No        | v1         |          |            |
|      | POST      | /api/todo                  | api.todo.store   | App\Api\V1\Controllers\TodoController@store                                                                                   | No        | v1         |          |            |
|      | GET|HEAD  | /api/todo/{todo}           | api.todo.show    | App\Api\V1\Controllers\TodoController@show                                                                                    | No        | v1         |          |            |
|      | PUT|PATCH | /api/todo/{todo}           | api.todo.update  | App\Api\V1\Controllers\TodoController@update                                                                                  | No        | v1         |          |            |
|      | DELETE    | /api/todo/{todo}           | api.todo.destroy | App\Api\V1\Controllers\TodoController@destroy                                                                                 | No        | v1         |          |            |
|      | GET|HEAD  | /api/test                  | api.test.index   | App\Api\V1\Controllers\TestsController@index@index                                                                            | No        | v1         |          |            |
|      | POST      | /api/test                  | api.test.store   | App\Api\V1\Controllers\TestsController@index@store                                                                            | No        | v1         |          |            |
|      | GET|HEAD  | /api/test/{test}           | api.test.show    | App\Api\V1\Controllers\TestsController@index@show                                                                             | No        | v1         |          |            |
|      | PUT|PATCH | /api/test/{test}           | api.test.update  | App\Api\V1\Controllers\TestsController@index@update                                                                           | No        | v1         |          |            |
|      | DELETE    | /api/test/{test}           | api.test.destroy | App\Api\V1\Controllers\TestsController@index@destroy                                                                          | No        | v1         |          |            |
+------+-----------+----------------------------+------------------+-----------------------------------------------------------------------------------------------------------------