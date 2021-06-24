---
title: 更新设置
description: '更新 settings 对象的属性。 '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: f776bd5ac5dad802a8c977cbe32842e619c74434
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107758"
---
# <a name="update-settings"></a>更新设置

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [userSettings 对象](../resources/usersettings.md) 的属性。 根据用户的偏好或组织策略，同一组织中用户可以具有不同的设置。 若要获取用户当前设置，请参阅 [当前用户设置](usersettings-get.md)。 


### <a name="batch-request"></a>批量请求

也可以选择退出通过批处理请求Delve用户。
若要了解更多信息，请参阅 [JSON 批处理](/graph/json-batching)。

>**重要** 提示：只有组织管理 [角色](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) 组的成员才能更新多个用户。 



## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadWrite、User.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | User.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

```http
PATCH /me/settings
```

具有“用户ID”或“userPrincipalName”的请求只能由用户或具有 User.ReadWrite.All 权限的用户访问。 若要了解详细信息，请参阅[权限](/graph/permissions-reference)。 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a>请求标头

| 标头       | 值|
|:-----------|:------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|布尔值|设置为 true 可禁止用户Office Delve文档。 此设置反映控件在[控件Office Delve。](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)|

## <a name="example"></a>示例 

##### <a name="request"></a>请求

下面是一个示例请求，请求如何选择退出用户Delve并禁用他针对整个组织的内容相关性的贡献。

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a>响应

这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```



