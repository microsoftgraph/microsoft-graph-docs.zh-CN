---
title: 创建 externalGroup
description: 创建新的 externalGroup 对象。
author: sacampbe-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: bd7a09ae83540ab739bdda97fcdbfc14827a7e25
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697500"
---
# <a name="create-externalgroup"></a>创建 externalGroup
命名空间：microsoft.graph.externalConnectors



创建新的 [externalGroup](../resources/externalconnectors-externalgroup.md) 对象。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持                               |
| 委派（个人 Microsoft 帐户） | 不支持                               |
| 应用程序                            | ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All                  |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /connections/{connectionsId}/groups
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
|:--------------|:----------------------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供 **externalGroup** 对象的 JSON 表示形式。

可以在创建 externalGroup 时指定 **以下属性**。

| 属性    | 类型   | 说明                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | 连接内外部组的唯一 ID。 它必须是字母数字，并且最多为 128 个字符。 必需。 |
| displayName | String | 外部组的友好名称。 可选。                                                                      |
| description | String | 外部组的说明。 可选。                                                                         |



## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 **externalGroup** 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_connection"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups
Content-Type: application/json

{
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
