---
title: 创建标识
description: 在 externalGroup 中创建新成员作为标识资源。
author: sacampbe
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 42ac3ef6dd3aa12d1116c09694c74957c34077e3
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697499"
---
# <a name="create-identity"></a>创建标识
命名空间：microsoft.graph.externalConnectors



为 [externalGroup](../resources/externalconnectors-identity.md) 中的新成员创建 [标识资源](../resources/externalconnectors-externalgroup.md)。

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
POST /connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
|:--------------|:----------------------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供标识对象的 JSON **表示** 形式。

为 **externalGroup** 中的成员创建 **标识** 资源时，可以指定以下属性。

| 属性       | 类型                    | 说明                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| id             | String                  | 成员 `id` 的唯一性。 对于用户 **或组**，它Azure Active Directory objectId，对于外部组，为 **externalGroupId。** 此为必需属性。                                    |
| type           | microsoft.graph.externalConnectors.identityType | 添加到外部组的成员的类型。 可能的值是 `user` `group` `externalGroup` ：、、。 必需。 |


## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 **identity** 对象。

## <a name="examples"></a>示例

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a>示例 1：将Azure Active Directory用户添加为成员

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_aad_user_identity_from_group"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user"
}
```

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.identity"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user"
}
```

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a>示例 2：将Azure Active Directory组添加为成员

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_aad_group_identity_from_group"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.identity"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group"
}
```

### <a name="example-3-add-another-external-group-as-a-member"></a>示例 3：将另一个外部组添加为成员

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_external_group_identity_from_group"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "1431b9c38ee647f6a",
  "type": "externalGroup",
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.identity"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "14m1b9c38qe647f6a",
  "type": "externalGroup"
}
```
