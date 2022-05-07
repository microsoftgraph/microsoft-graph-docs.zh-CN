---
title: 获取用户的增量更改
description: Microsoft Graph中的增量查询可用于查询支持的资源的添加、删除或更新。 它通过一系列增量请求启用。 对于用户，增量查询使你可以发现更改，而无需提取用户组来比较更改。
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: d03762372a789d76d3f38121da47d662e281b2f2
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247222"
---
# <a name="get-incremental-changes-for-users"></a>获取用户的增量更改

Microsoft Graph中的 [增量查询](./delta-query-overview.md)，可用于查询 [支持的资源](delta-query-overview.md#supported-resources) 的添加、删除或更新。 它通过一系列 [增量](/graph/api/user-delta) 请求启用。 对于用户，增量查询使你可以发现更改，而无需提取用户组来比较更改。

以后，对本地配置文件存储使用同步用户功能的客户端可以将增量查询用于初始完全同步和后续增量同步。通常，客户会对租户中的所有用户进行初始完全同步，之后定期获取对用户的增量更改。

## <a name="track-changes-to-users"></a>获取对用户的更改

使用 **增量** 函数通过一个或多个 GET 请求跟踪用户更改。 GET 请求类似于 [列表用户](/graph/api/user-list) 请求，但 URL 中包含以下额外对象除外:

- **delta** 函数。
- 上一个 GET **delta** 函数调用的 [状态令牌](./delta-query-overview.md)（_deltaToken_ 或 _skipToken_）。

## <a name="example-to-track-changes-to-users"></a>跟踪用户更改的示例

下面的示例演示了一系列跟踪用户更改的请求:

1. [初始请求](#initial-request) 和 [响应](#initial-response)
2. [nextLink 请求](#nextlink-request) 和 [响应](#nextlink-response)
3. [最终的 nextLink 请求](#final-nextlink-request) 和 [响应](#final-nextlink-response)
4. [deltaLink 请求](#deltalink-request) 和 [deltaLink 响应](#deltalink-response)

在响应中记下以下内容:

- 如果用户遭删除，项中包含注释：`@removed` 值为 `"reason": "changed"`。
- 如果用户遭永久删除，项中包含注释: `@removed` 值为 `"reason": "deleted"`。
- 如果创建或恢复用户，则没有注释。

### <a name="initial-request"></a>初始请求

若要跟踪用户资源中的更改，请发出请求，并将 **增量** 函数作为 URL 段。

记下以下各项:

- 请求中包含可选的 `$select` 查询参数，以演示如何在以后的请求中自动包含查询参数。
- 初始请求不包括状态令牌。状态令牌将用于后续请求中。

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

### <a name="initial-response"></a>初始响应

如果成功，此方法的响应正文返回`200 OK`响应代码和[用户](/graph/api/resources/user)集合对象。假定整组用户过大，则响应还将包含 `@odata.nextLink` 参数中的 `@odata.nextLink` 状态令牌。

本示例中，返回 `@odata.nextLink` URL，表示此会话存在要检索的其他数据页面。初始请求的 `$select` 查询参数已编码为 `@odata.nextLink` URL。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,givenName,surname)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa",
  "value": [
    {
      "displayName":"Cameron White",
      "givenName":"Cameron",
      "surname":"White",
      "id":"ffff7b1a-13b6-477b-8c0c-380905cd99f7"
    },
    {
      "displayName":"Delia Dennis",
      "givenName":"Delia",
      "surname":"Dennis",
      "id":"605d1257-ffff-40b6-8e6f-528a53f5dc55"
    },
    {
      "id": "86462606-fde0-4fc4-9e0c-a20eb73e54c6",
      "@removed": {
        "reason": "deleted"
      }
    },
    {
      "displayName": "Conf Room Adams",
      "id": "6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0"
    }
  ]
}
```

### <a name="nextlink-request"></a>nextLink 请求

第二个请求指定上一个响应中返回的 `skipToken`。请注意，`$select` 参数已编码并包含在 `skipToken`  中。

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

### <a name="nextlink-response"></a>nextLink 响应

响应包含另一个`@odata.nextLink`，其中有一个新的`skipToken`值，这表示为用户跟踪的更多更改可用。 在更多请求中使用 `@odata.nextLink` URL，直到在最终响应中返回 `@odata.deltaLink` URL (在 `@odata.deltaLink` 参数中)。 即使值为空数组也是如此。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Mallory Cortez",
      "givenName":"Mallory",
      "surname":"Cortez",
      "id":"d8c37826-ffff-4cae-b348-e2725b1e814b"
    },
    {
      "displayName":"Diego Sicilian",
      "givenName":"Diego",
      "surname":"Sicilian",
      "id":"8b1ee412-cd8f-4d59-ffff-24010edb9f1f"
    }
  ]
}
```

### <a name="final-nextlink-request"></a>最终 nextLink 请求

第三个请求使用上次同步请求返回的最新 `skipToken`。 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

### <a name="final-nextlink-response"></a>最终 nextLink 响应

当返回 `@odata.deltaLink` URL 时，不再返回关于用户对象现有状态的数据。为了执行以后的请求，应用程序使用 `@odata.deltaLink` URL 了解用户的其他更改。保存 `deltaToken`，并在后续请求 URL 中使用它来发现用户的更多更改。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Lidia Holloway",
      "givenName":"Lidia",
      "surname":"Holloway",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "displayName":"Patti Fernandez",
      "givenName":"Patti",
      "surname":"Fernandez",
      "id":"f6ede700-27d0-4c42-bfb9-4dffff43c74a"
    }
  ]
}
```

### <a name="deltalink-request"></a>deltaLink 请求

使用 [ 上次响应 ](#final-nextlink-response) 中的 `deltaToken`，将收到自上次请求以来用户的更改 (添加、删除或更新)。

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a>deltaLink 响应

如果未发生任何更改，则返回 `@odata.deltaLink` 而不返回结果 - **值** 属性为空数组。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": []
}
```

如果发生更改，则包含已更改用户对象的集合。 响应还包含 `@odata.nextLink` 或 `@odata.deltaLink`（如果要检索多个更改页面）。 实现遵循 `@odata.nextLink` 的相同模式，并为将来的调用保留最终 `@odata.deltaLink`。

>**注意：** 此请求可能对最近创建、更新或删除的用户具有复制延迟。 请在一段时间后重试 `@odata.nextLink` 或 `@odata.deltaLink` 以检索最新更改。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": [
    {
      "displayName":"MOD Administrator",
      "givenName":"MOD",
      "surname":"Administrator",
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

## <a name="see-also"></a>另请参阅
+ [Microsoft Graph delta 查询](delta-query-overview.md)概述。
