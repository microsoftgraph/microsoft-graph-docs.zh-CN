---
title: 获取用户的增量更改
description: Delta 查询可通过调用一系列 delta 函数查询用户的添加、删除或更新。Delta 查询使你无需读取 Microsoft Graph 的整组用户就能够发现用户的更改并进行比较。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: b4f79951f79393e22c40ef9a4f55e29e0145ccea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526333"
---
# <a name="get-incremental-changes-for-users"></a>获取用户的增量更改

[Delta 查询](./delta-query-overview.md)可通过调用一系列 [delta](/graph/api/user-delta?view=graph-rest-1.0) 函数查询用户的添加、删除或更新。Delta 查询使你无需读取 Microsoft Graph 的整组用户就能够发现用户的更改并进行比较。

以后，对本地配置文件存储使用同步用户功能的客户端可以将增量查询用于初始完全同步和增量同步。通常，客户会对租户中的所有用户进行初始完全同步，之后定期获取对用户的增量更改。

## <a name="tracking-user-changes"></a>跟踪用户更改

跟踪用户更改是发出 **delta** 函数的一个或多个 GET 请求。发出 GET 请求与[列出用户](/graph/api/user-list?view=graph-rest-1.0)的方式非常相似，除了要包括以下内容：

- **delta** 函数。
- 上一个 GET **delta** 函数调用的[状态令牌](./delta-query-overview.md)（_deltaToken_ 或 _skipToken_）。

## <a name="example"></a>示例

以下示例显示了跟踪用户更改的一系列请求：

1. [初始请求](#initial-request)和[响应](#initial-response)
2. [nextLink 请求](#nextlink-request)和[响应](#nextlink-response)
3. [最终 nextLink 请求](#final-nextlink-request)和[响应](#final-nextlink-response)
4. [deltaLink 请求](#deltalink-request)和 [deltaLink 响应](#deltalink-response)

## <a name="initial-request"></a>初始请求

为开始跟踪用户资源的更改，请在用户资源上发出包含 delta 函数的请求。

请注意以下事项：

- 请求中包含可选的 $select 查询参数，以演示如何在以后的请求中自动包含查询参数。
- 初始请求不包括状态令牌。状态令牌将用于后续请求中。

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

## <a name="initial-response"></a>初始响应

如果成功，此方法的响应正文返回`200 OK`响应代码和[用户](/graph/api/resources/user?view=graph-rest-1.0)集合对象。假定整组用户过大，则响应还将包含 nextLink 状态令牌。

本示例中，返回 nextLink URL，表示此会话存在要检索的其他数据页面。初始请求的 $select 查询参数已编码为 nextLink URL。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,givenName,surname)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa",
  "value": [
    {
      "displayName":"Testuser1",
      "givenName":"John",
      "surname":"Doe",
      "id":"ffff7b1a-13b6-477b-8c0c-380905cd99f7"
    },
    {
      "displayName":"Testuser2",
      "givenName":"Jane",
      "surname":"Doe",
      "id":"605d1257-ffff-40b6-8e6f-528a53f5dc55"
    }
  ]
}
```

## <a name="nextlink-request"></a>nextLink 请求

第二个请求指定上一个响应中返回的 `skipToken`。请注意不需要 `$select` 参数，因为 `skipToken` 已将其编码且包含其中。

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

## <a name="nextlink-response"></a>nextLink 响应

该响应包含 `nextLink` 和另一个 `skipToken`，表示存在更多可用的用户。继续使用 nextLink URL 发出请求，直到响应中返回 deltaLink URL。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Testuser3",
      "givenName":"Pat",
      "surname":"Doe",
      "id":"d8c37826-ffff-4cae-b348-e2725b1e814b"
    },
    {
      "displayName":"Testuser4",
      "givenName":"Meghan",
      "surname":"Doe",
      "id":"8b1ee412-cd8f-4d59-ffff-24010edb9f1f"
    }
  ]
}
```

## <a name="final-nextlink-request"></a>最终 nextLink 请求

第三个请求继续使用上次同步请求返回的最新 `skipToken`。 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhaOYDE2VPA4vxIPA90-P6OzGd6Rvku5fDgBRIGS
```

## <a name="final-nextlink-response"></a>最终 nextLink 响应

当返回 deltaLink URL 时，不再返回关于资源现有状态的数据。为了执行以后的请求，应用程序使用 deltaLink URL 了解资源更改。保存 `deltaToken`，并在请求 URL 中使用它来发现用户更改。 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser5",
      "givenName":"Al",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "displayName":"Testuser6",
      "givenName":"Sam",
      "surname":"Doe",
      "id":"f6ede700-27d0-4c42-bfb9-4dffff43c74a"
    }
  ]
}
```

## <a name="deltalink-request"></a>deltaLink 请求

通过使用[上次响应](#final-nextlink-response)中的 `deltaToken`，你将能够获取上次请求以来的已更改用户（添加、删除或更新）。

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a>deltaLink 响应

如果未发生更改，则会返回同一 `deltaToken` 且无返回结果。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": []
}
```

如果发生更改，便会返回相同的 `deltaToken`，其中包括已更改用户的集合。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser7",
      "givenName":"Joe",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "id":"8ffff70c-1c63-4860-b963-e34ec660931d",
      "@removed": {
         "reason": "changed"
      }
    }
  ]
}
```

上面示例响应的一些注意事项如下：

- 如果用户遭删除，项中包含注释：`@removed` 值为 `"reason": "changed"`。

- 如果用户遭永久删除，项中包含注释：`@removed` 值为 `"reason": "deleted"`。

- 如果用户被创建或恢复，则没有注释。

## <a name="see-also"></a>另请参阅
[Microsoft Graph delta 查询](delta-query-overview.md)概述。
