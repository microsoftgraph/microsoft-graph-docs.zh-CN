---
title: 获取组的增量更改
description: Delta 查询允许你通过一系列 Delta 函数调用来查询对组的添加、删除或更新。Delta 查询可便于发现组的更改
author: davidmu1
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: cea4e335a02c2ebdf107cdfbca72072b0b18d2f3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142385"
---
# <a name="get-incremental-changes-for-groups"></a>获取组的增量更改

[Delta 查询](./delta-query-overview.md)可通过调用一系列的 [delta](/graph/api/group-delta?view=graph-rest-1.0) 函数来查询组的添加、删除或更新。增量查询使你无需读取 Microsoft Graph 的整个组就能够发现组的更改并进行比较。

以后，对本地配置文件存储使用同步组功能的客户端可以将增量查询用于初始完全同步和增量同步。通常，客户会对租户中的所有组进行初始完全同步，之后定期获取对组的增量更改。

## <a name="tracking-group-changes"></a>跟踪组更改

跟踪组更改是发出 **delta** 函数的一个或多个 GET 请求。发出 GET 请求与 [列出组](/graph/api/group-list?view=graph-rest-1.0)的方式非常相似，除了要包括以下内容：

- **delta** 函数。
- 上一个 GET **delta** 函数调用的 [状态令牌](./delta-query-overview.md)（*deltaToken* 或 *skipToken*）。

## <a name="example"></a>示例

以下示例显示跟踪组更改的一系列请求：

1. [初始请求](#initial-request)和[响应](#initial-response)
2. [nextLink 请求](#nextlink-request)和[响应](#nextlink-response)
3. [最终 nextLink 请求](#final-nextlink-request)和[响应](#final-nextlink-response)
4. [deltaLink 请求](#deltalink-request)和 [deltaLink 响应](#deltalink-response)

## <a name="initial-request"></a>初始请求

为开始跟踪组资源的更改，请在组资源上发出包含 delta 函数的请求。

请注意以下几点：

- 请求中包含可选的 `$select` 查询参数，以演示如何在以后的请求中自动包含查询参数。
- 可选的 `$select` 查询参数还用于显示如何一起检索组成员和组对象。 这允许跟踪成员身份变更，例如当用户被添加到组或从组中删除时。
- 初始请求不包括状态令牌。状态令牌将用于后续请求中。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

## <a name="initial-response"></a>初始响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和[组](/graph/api/resources/group?view=graph-rest-1.0)集合对象。 如果整个组集过大而无法适应一个响应，那么还将包括一个包含状态令牌的 `nextLink`。

此示例中包含 `nextLink`；原始 `$select` 查询参数则在状态令牌中进行了编码。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

>**注意：**`members@delta` 属性包含在第一个组对象 (TestGroup1) 中并包含该组的两个当前成员。 TestGroup2 不包含此属性，因为组中没有任何成员。

## <a name="nextlink-request"></a>nextLink 请求

第二个请求使用上一个响应中的 `nextLink`，其中包含 `skipToken`。 请注意，`$select` 参数不显式出现，因为它在令牌中编码。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a>nextLink 响应

该响应包含另一个带新 `skipToken` 值的 `nextLink`，它表示存在更多可用的组。 应使用 `nextLink` URL 继续发出请求，直到在最终响应中返回 `deltaLink` URL，即使该值为空数组（在某些情况下可能会出现此情况）。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "3c8ac7c4-d365-4df9-abfa-356a9dd7763c"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

## <a name="final-nextlink-request"></a>最终 nextLink 请求

第三个请求再次使用最新的 `nextLink`。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>最终 nextLink 响应

最后返回 `deltaLink` URL，这意味着没有更多数据反映现有的组状态。 对于将来请求，应用程序将使用它所包含的 `deltaLink` 和 `deltaToken` 值来了解有关组的新更改。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
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

通过使用[上次响应](#final-nextlink-response)的 `deltaLink`，你将能够获取自上次请求以来对组所做的新更改。更改包括：
- 新创建的组对象。
- 已删除的组对象。
- 属性已更改的组对象（例如，修改了 **displayName**）。
- 已为其添加或移除成员对象的组对象。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a>deltaLink 响应

如果未发生更改，则会返回 `deltaLink` 且无返回结果 - `value` 属性为空。 请确保将应用程序中的以前链接替换为新链接以便在日后调用中使用。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

如果发生更改，则包含已更改组的集合。 响应还包含 `nextLink` 或 `deltaLink`（如果要检索多个更改页面）。 应像以前一样实现遵循 `nextLinks` 的相同模式，并保留最终的 `deltaLink` 供日后调用。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
          {
              "displayName": "TestGroup3",
              "description": "A test group for change tracking",
              "id": "2e5807ce-58f3-4a94-9b37-ffff2e085957",
              "members@delta": [
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
                      "@removed": {
                          "reason": "deleted"
                      }
                  },
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "37de1ae3-408f-4702-8636-20824abda004"
                  }
              ]
          }
      ]
}
```

上面示例响应的一些注意事项如下：

- 这些对象连同一组相同的属性一起返回，这些属性最初通过 `$select` 查询参数指定。

- 同时包括已更改和未更改的属性。在上述示例中，`description` 属性具有新值，而 `displayName` 属性未发生更改。

- `members@delta` 包含对成员身份的任何更改。

  - 列表中的第一个用户已经从组中删除 - 要么删除成员身份，要么删除用户对象本身。 `@removed` 属性对此进行了说明。 只有被永久删除的用户才会从组中删除。 临时删除的用户保留自己的组成员资格，除非被永久删除，否则不会显示在增量结果中。 有关详细信息，请参阅[目录（已删除的项）](/graph/api/resources/directory?view=graph-rest-1.0)。

  - 第二个用户已添加到组。

## <a name="paging-through-members-in-a-large-group"></a>逐页查看大型组中的成员

当未指定 `$select` 查询参数，或已显式指定 `$select=members` 参数时，`members@delta` 属性默认包含在组对象中。 对于包含许多成员的组来说，可能所有成员都无法适应单个响应；在本节中，我们将介绍为处理这种情况所应实现的模式。

>**注意：** 此模式既适用于组状态的初始检索，也适用于后续调用，以获取增量更改。

假定正在执行以下增量查询 - 要捕获组的初始完整状态，或要在稍后获取增量更改：

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

1. Microsoft Graph 可能返回一个仅包含一个组对象的响应，其中 `members@delta` 属性中有一个大型成员列表：

**第一页**

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "37de1ae3-408f-4702-8636-20824abda004"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

2. 如果按照 `nextLink` 操作，可能会再次收到包含同一组对象的响应。 将返回相同的属性值，但 `members@delta` 属性现在包含不同的用户列表。

**第二页**

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "c08a463b-7b8a-40a4-aa31-f9bf690b9551",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "23423fa6-821e-44b2-aae4-d039d33884c2"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

3. 最终，将以此方式返回整个成员列表，并且其他组将开始在响应中显示。

建议使用以下最佳做法来正确处理此模式：
- 始终按照 `nextLink` 操作，并在本地合并每个组的状态：当收到与同一个组相关的响应时，使用它们在应用程序中构建完整的成员身份列表。
- 最好不要假定响应的特定顺序。 假设同一组可以显示在 `nextLink` 序列的任意位置，并以合并逻辑进行处理。


## <a name="see-also"></a>另请参阅
[Microsoft Graph delta 查询](delta-query-overview.md)概述。
