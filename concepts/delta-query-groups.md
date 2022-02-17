---
title: 获取组的增量更改
description: Microsoft Graph中的增量查询可用于查询支持的资源的添加、删除或更新。 它通过一系列增量请求启用。 对于组，增量查询使你可以发现更改，而无需提取整组来比较更改。
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: c7e336d4bcfe0de5d64153c50ede0d8008a17708
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878741"
---
# <a name="get-incremental-changes-for-groups"></a>获取组的增量更改

Microsoft Graph中的[增量查询](./delta-query-overview.md)，可用于查询[支持的资源](delta-query-overview.md#supported-resources)的添加、删除或更新。 它通过一系列 [增量](/graph/api/group-delta?) 请求启用。 对于组，增量查询使你可以发现更改，而无需提取整组来比较更改。

将组与本地配置文件存储同步的客户端可以使用增量查询进行初始完全同步以及后续增量同步。 通常，客户端会对租户中的所有组进行初始完全同步，然后定期获取对组的增量更改。

## <a name="track-changes-to-groups"></a>跟踪对组的更改

使用 **增量** 函数通过一个或多个 GET 请求跟踪组更改。 GET 请求类似于 [列表组](/graph/api/group-list?) 请求，但 URL 中包含以下额外对象除外：

- **delta** 函数。
- 上一个 GET **delta** 函数调用的 [状态令牌](./delta-query-overview.md)（_deltaToken_ 或 _skipToken_）。

## <a name="example-to-track-changes-to-groups"></a>跟踪组更改的示例

以下示例显示跟踪组更改的一系列请求：

1. [初始请求](#initial-request)和[响应](#initial-response)
2. [nextLink 请求](#nextlink-request)和[响应](#nextlink-response)
3. [最终 nextLink 请求](#final-nextlink-request)和[响应](#final-nextlink-response)
4. [deltaLink 请求](#deltalink-request)和 [deltaLink 响应](#deltalink-response)


下面的示例演示了一系列跟踪组更改的请求：

1. [初始请求](#initial-request)和[响应](#initial-response)
2. [nextLink 请求](#nextlink-request)和[响应](#nextlink-response)
3. [最终的 nextLink 请求](#final-nextlink-request)和[响应](#final-nextlink-response)
4. [deltaLink 请求](#deltalink-request)和[deltaLink 响应](#deltalink-response)

在响应中记下以下内容：

- 删除组（Microsoft 365组）时，项包含批注： `@removed` 值为 `"reason": "changed"`。
- 永久删除组（安全组或 [永久删除Microsoft 365组](/graph/api/directory-deleteditems-list.)）时，项将包含一个批注： `@removed` 值为 `"reason": "deleted"`。
- 创建或还原组时，没有批注。

### <a name="initial-request"></a>初始请求

若要跟踪组资源中的更改，请发出请求，并将 **增量** 函数作为 URL 段。

记下以下各项：

- 请求中包含可选的 `$select` 查询参数，以演示如何在以后的请求中自动包含查询参数。
- 可选的 `$select` 查询参数还用于显示如何一起检索组成员和组对象。 这允许跟踪成员身份变更，例如当用户被添加到组或从组中删除时。
- 初始请求不包括状态令牌。 状态令牌将用于后续请求中。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

### <a name="initial-response"></a>初始响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和[组](/graph/api/resources/group)集合对象。 如果整个组集过大而无法适应一个响应，那么还将包括一个包含状态令牌的 `nextLink`。

此示例中包含 `nextLink`；原始 `$select` 查询参数则在状态令牌中进行了编码。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"All Company",
      "description":"This is the default group for everyone in the network",
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
      "displayName":"sg-HR",
      "description":"All HR personnel",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

>**注意：** " `members@delta` "属性包含在第一个组对象（ **"所有公司"** ）中，并且包含该组的两个当前成员。 **sg-HR** 不包含该属性，因为该组没有任何成员。

### <a name="nextlink-request"></a>nextLink 请求

第二个请求使用上一个响应中的 `nextLink`，其中包含 `skipToken`。 请注意，`$select`参数在编码并包含在令牌中时并不明显存在。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

### <a name="nextlink-response"></a>nextLink 响应

响应包含另一个`nextLink`，其中有一个新的`skipToken`值，这表示为组跟踪的更多更改可用。 在更多请求中使用 `nextLink` URL，直到在最终响应中返回`deltaLink` URL（在 `@odata.deltaLink` 参数中）。 即使值为空数组也是如此。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Mark 8 Project Team",
      "description":"Mark 8 Project Team",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"Sales and Marketing",
      "description":"Sales and Marketing",
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

### <a name="final-nextlink-request"></a>最终 nextLink 请求

第三个请求使用上次同步请求返回的最新`nextLink`。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

### <a name="final-nextlink-response"></a>最终 nextLink 响应

返回 `deltaLink` URL 时，不再有有关组对象的现有状态的数据。  对于将来的请求，应用程序使用 `deltaLink` URL 了解组的其他更改。 保存 `deltaToken`并在后续请求 URL 中使用它来发现对组的更多更改。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"All Employees",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"Remote living",
      "description":"Remote living",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

### <a name="deltalink-request"></a>deltaLink 请求

使用[上次响应](#final-nextlink-response)中的`deltaLink`，你将收到自上次请求以来组的更改（添加、删除或更新）。 这些更改包括：

- 新创建的组对象。
- 已删除的组对象。
- 已更改属性的组对象（例如，已修改 **displayName** ）。
- 已为其添加或移除成员对象的组对象。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

### <a name="deltalink-response"></a>deltaLink 响应

如果未发生任何更改，则返回 `deltaLink` 而不返回结果 - **值** 属性为空数组。 请确保将应用程序中的以前链接替换为新链接以便在日后调用中使用。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

如果发生更改，则包含已更改组的集合。 响应还包含 `nextLink` 或 `deltaLink`（如果要检索多个更改页面）。 实现遵循 `nextLink` 的相同模式，并为将来的调用保留最终 `deltaLink`。

>**注意：** 此请求可能对最近创建、更新或删除的组具有复制延迟。 请在一段时间后重试 `nextLink` 或 `deltaLink`以检索最新更改。

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

- 同时包括更改和未更改的属性。 在上面的示例中， `description` 属性有一个新值，而 `displayName` 属性没有更改。

- `members@delta`包含对组成员身份的以下更改。

  - 列表中的第一个用户已经从组中删除 - 要么删除成员身份，要么删除用户对象本身。 `@removed` 属性对此进行了说明。 只有被永久删除的用户才会从组中删除。 已临时删除的用户保留其组成员身份，并且在永久删除之前不会出现在增量结果中。 有关详细信息，请参阅[目录（已删除的项）](/graph/api/resources/directory)。

  - 第二个用户已添加到组。

## <a name="paging-through-members-in-a-large-group"></a>逐页查看大型组中的成员

默认情况下，当未指定`$select`查询参数或显式指定`$select=members`参数时，`members@delta` 属性包含在组对象中。 对于具有多个成员的组，可能所有成员都无法适应单个响应。 实现以下模式来处理此类情况。

>**注意：** 此模式既适用于组状态的初始检索，也适用于后续调用，以获取增量更改。

假设运行以下增量查询 - 捕获组的初始完整状态，或稍后获取增量更改：

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

2. 遵循 `nextLink`时，可能会收到包含同一组对象的响应。 将返回相同的属性值，但 `members@delta` 属性现在包含不同的用户列表。

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
- 不要假定特定的响应序列。 假设同一组可以显示在 `nextLink` 序列的任意位置，并以合并逻辑进行处理。


## <a name="see-also"></a>另请参阅
[Microsoft Graph delta 查询](delta-query-overview.md)概述。
