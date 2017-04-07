# <a name="get-incremental-changes-for-groups-preview"></a>获取组的增量更改（预览）

[Delta 查询](./delta_query_overview.md)可通过调用一系列的 [delta](../api-reference/beta/api/group_delta.md) 函数来查询组的添加、删除或更新。增量查询使你无需读取 Microsoft Graph 的整个组就能够发现组的更改并进行比较。

Delta 查询支持检索租户中所有组的完全同步，以及仅检索自上次同步以来已更改组的增量同步。通常，需要对租户中的所有组进行初始完全同步，之后可定期获取组的增量更改。 

## <a name="tracking-group-changes"></a>跟踪组更改

跟踪组更改是发出 **delta** 函数的一个或多个 GET 请求。发出 GET 请求与[列出组](../api-reference/beta/api/group_list.md)的方式非常相似，除了要包括以下内容：

- **delta** 函数。
- 上一个 GET **delta** 函数调用的[状态令牌](./delta_query_overview.md)（_deltaToken_ 或 _skipToken_）。

## <a name="example"></a>示例

以下示例显示跟踪组更改的一系列请求：

1. [初始请求](#initial-request)和[响应](#initial-response)
2. [nextLink 请求](#nextlink-request)和[响应](#nextlink-response)
3. [最终 nextLink 请求](#final-nextlink-request)和[响应](#final-nextlink-response)
4. [deltaLink 请求](#deltalink-request)和 [deltaLink 响应](#deltalink-response)

## <a name="initial-request"></a>初始请求

为开始跟踪组资源的更改，请在组资源上发出包含 delta 函数的请求。 

请注意以下事项：

- 请求中包含可选的 $select 查询参数，以演示如何在以后的请求中自动包含查询参数。
- 初始请求不包括状态令牌。状态令牌将用于后续请求中。

``` http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description
```

### <a name="initial-response"></a>初始响应

如果成功，此方法在响应正文中返回 `200, OK` 响应代码和[组](../api-reference/beta/resources/group.md)集合对象。假如整个组过大，则响应还将包含 nextLink 状态令牌。

本示例中，返回 nextLink URL，表示此会话存在要检索的其他数据页面。初始请求的 $select 查询参数已编码为 nextLink URL。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff"
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

## <a name="nextlink-request"></a>nextLink 请求

第二个请求指定上一个响应中返回的 `skipToken`。请注意不需要 `$select` 参数，因为 `skipToken` 已将其编码且包含其中。

``` http
GET https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a>nextLink 响应

该响应包含 `nextLink` 和另一个 `skipToken`，表示存在更多可用的组。继续使用 nextLink URL 发出请求，直到响应中返回 deltaLink URL。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957"
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505"
    }
  ]
}
```

## <a name="final-nextlink-request"></a>最终 nextLink 请求

第三个请求继续使用上次同步请求返回的最新 `skipToken`。 

``` http
GET https://graph.microsoft.com/beta/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>最终 nextLink 响应

当返回 deltaLink URL 时，不再返回关于资源现有状态的数据。为了执行以后的请求，应用程序使用 deltaLink URL 了解资源更改。保存 `deltaToken`，并在请求 URL 中使用它来发现组更改。 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup5",
      "description":"Employees in test group 5",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"TestGroup6",
      "description":"Employees in test group 6",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

## <a name="deltalink-request"></a>deltaLink 请求

通过使用[上次响应](#final-nextlink-response)的 `deltaToken`，你将能够获取自上次请求以来的已更改组（添加、删除或更新）。

``` http
GET https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a>deltaLink 响应

如果未发生更改，则会返回同一 `deltatoken` 且无返回结果。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

如果发生更改，则会返回同一 `deltatoken`，包括已更改组的集合。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup7",
      "description":"Employees in test group 7",
      "id":"f764235c-ffff-4843-a14a-1d8826967260"
    }
  ]
}
```

## <a name="see-also"></a>另请参阅
[Microsoft Graph delta 查询](../concepts/delta_query_overview.md)概述。