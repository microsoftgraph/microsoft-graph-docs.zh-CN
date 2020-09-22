---
title: 创建 externalGroupMember
description: 创建新的 externalGroupMember 对象。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c66c21e4b0842df4fb7ececa3378249347f3002d
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193845"
---
# <a name="create-externalgroupmember"></a>创建 externalGroupMember

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [externalGroupMember](../resources/externalgroupmember.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最高特权到最低特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持                               |
| 委派（个人 Microsoft 帐户） | 不支持                               |
| 应用程序                            | ExternalItem.ReadWrite.All                  |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
|:--------------|:----------------------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [externalGroupMember](../resources/externalgroupmember.md) 对象的 JSON 表示形式。

下表显示创建 [externalGroupMember](../resources/externalgroupmember.md)时所需的属性。

| 属性       | 类型                    | 说明                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| id             | 字符串                  | 成员的唯一 `id` 。 在 Azure Active Directory 用户或组以及外部组的情况下，它将是 externalGroupId 的 objectId。                                    |
| type           | externalGroupMemberType | 添加到外部组的成员类型。 可能的值为： `user` 或者 `group` 当 identitySource 是 `azureActiveDirectory` identitySource 时， `group` `external` 则为。 |
| identitySource | identitySourceType      | 成员所属的标识源。 可取值为：`azureActiveDirectory`、`external`。                                                                                         |

## <a name="response"></a>响应

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [externalGroupMember](../resources/externalgroupmember.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a>示例1：将 Azure Active Directory 用户添加为成员

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a>示例2：将 Azure Active Directory 组添加为成员

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-3-add-another-external-group-as-a-member"></a>示例3：将另一个外部组添加为成员

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "1431b9c38ee647f6a",
  "type": "group",
  "identitySource": "external"
}
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "14m1b9c38qe647f6a",
  "type": "group",
  "identitySource": "external"
}
```
