---
title: directoryObject：checkMemberGroups
description: 检查指定组列表中的成员身份，然后从该列表返回指定的用户、组、服务主体、组织联系人或目录对象是其成员的组。
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 04696e05b0c3c64bbc8a6fe49437bdbbf7db3ccd
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2021
ms.locfileid: "61124124"
---
# <a name="directoryobject-checkmembergroups"></a>directoryObject：checkMemberGroups

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检查指定组列表中的成员身份，然后从该列表返回指定的[用户](../resources/user.md)、组、服务主体、组织联系人或[目录](../resources/directoryobject.md)对象[](../resources/group.md)是其成员[](../resources/serviceprincipal.md)的组。 [](../resources/orgcontact.md) 此函数是可传递的。

每个请求最多可检查 20 个组。 此函数支持在 Azure AD 中设置的所有组。 由于Microsoft 365组不能包含其他组，因此Microsoft 365组的成员始终是直接的。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="group-memberships-for-a-directory-object"></a>目录对象的组成员身份

| 权限类型                        | 权限（从最低特权到最高特权）           |
|:---------------------------------------|:------------------------------------------------------|
| 委派（工作或学校帐户）     | User.ReadBasic.All、User.Read.All、Directory.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                        |
| 应用程序                            | User.Read.All、Directory.Read.All                     |

### <a name="group-memberships-for-a-user"></a>用户的组成员身份

| 权限类型 | 权限（从最低特权到最高特权） |
|:-|:-|
| 委派（工作或学校帐户） | User.ReadBasic.All、User.Read.All、Directory.Read.All、User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | User.Read.All、Directory.Read.All、User.ReadWrite.All、Directory.ReadWrite.All |

### <a name="group-memberships-for-a-group"></a>组的组成员身份

| 权限类型 | 权限（从最低特权到最高特权） |
|:-|:-|
| 委派（工作或学校帐户） | GroupMember.Read.All、Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All |

### <a name="group-memberships-for-a-service-principal"></a>服务主体的组成员身份

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All |

### <a name="group-memberships-for-an-organizational-contact"></a>组织联系人的组成员身份

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Directory.Read.All、Directory.ReadWrite.All |

<!--
The following table lists the permission types to use for different scenarios.

| Scenario | Permissions |
|:-|:-|
| To get group memberships for the signed-in user | Use one of the following sets of permissions: <br/> <li> **User.Read** and **GroupMember.Read.All** <li>**User.Read** and **Group.Read.All** |
| To get group memberships for any user | Use one of the following sets of permissions: <br/> <li> **User.ReadBasic.All** and **GroupMember.Read.All** <li>**User.Read.All** and **GroupMember.Read.All** <li>**User.ReadBasic.All** and **Group.Read.All** <li>**User.Read.All** and **Group.Read.All** |
| To get group memberships for a group | Use either the **GroupMember.Read.All** or **Group.Read.All** permission. |
| To get group memberships for a service principal | Use one of the following sets of permissions <br/> <li>**Application.ReadWrite.All** and **GroupMember.Read.All** <li>**Application.ReadWrite.All** and **Group.Read.All** |
| To get group memberships for a directory object | Use the **Directory.Read.All** permission. |
-->

## <a name="http-request"></a>HTTP 请求

目录对象的组成员身份 (、组、服务主体或组织联系人) 。
<!-- { "blockType": "ignored" } -->
```http
POST /directoryObjects/{id}/checkMemberGroups
```

已登录用户或其他用户的组成员身份。
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
```

组的组成员身份。
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/checkMemberGroups
```

服务主体的组成员身份。
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups
```

组织联系人的组成员身份。
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups
```

## <a name="request-headers"></a>请求标头

| 名称       |说明|
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。 |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|groupIds|String collection |包含检查成员身份的组中的对象 ID 的集合。可以指定多达 20 个组。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。

## <a name="examples"></a>示例

### <a name="example-1-check-group-memberships-for-a-directory-object"></a>示例 1：检查目录对象的组成员身份

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/directoryObjects/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e/checkMemberGroups
Content-type: application/json

{
    "groupIds": [
        "f448435d-3ca7-4073-8152-a1fd73c0fd09",
        "bd7c6263-4dd5-4ae8-8c96-556e1c0bece6",
        "93670da6-d731-4366-94b5-abed40b6016b",
        "f5484ab1-4d4d-41ec-a9b8-754b3957bfc7",
        "c9103f26-f3cf-4004-a611-2a14e81b8f79"
    ]
}
```

#### <a name="response"></a>响应

下面是一个响应示例

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "f448435d-3ca7-4073-8152-a1fd73c0fd09",
        "93670da6-d731-4366-94b5-abed40b6016b",
        "f5484ab1-4d4d-41ec-a9b8-754b3957bfc7",
        "c9103f26-f3cf-4004-a611-2a14e81b8f79"
    ]
}
```

### <a name="example-2-check-group-memberships-for-the-signed-in-user"></a>示例 2：检查已登录用户的组成员身份

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups_me"
}-->
```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```


#### <a name="response"></a>响应
下面是一个响应示例

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


