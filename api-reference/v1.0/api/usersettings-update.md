---
title: 更新设置
description: '更新 settings 对象的属性。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e490a990344d27a5672b72466815b2754c3cb1fc
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844353"
---
# <a name="update-settings"></a>更新设置

更新[userSettings](../resources/usersettings.md)对象的属性。 同一个组织中的用户可以根据自己的首选项或组织策略拥有不同的设置。 若要获取用户的当前设置，请参阅[当前用户设置](usersettings-get.md)。 

### <a name="batch-request"></a>批量请求

此外，还可以从 Delve 中自愿退出多个用户，并通过批处理请求禁用对整个组织的内容关联的贡献。
若要了解详细信息，请参阅[JSON 批处理](https://developer.microsoft.com/graph/docs/concepts/json_batching)。

>**重要说明**：只有[组织管理](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US)角色组的成员才能更新多个用户。 



## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 所有用户读写。   |
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
|contributionToContentDiscoveryDisabled|布尔值|设置为 true 确实禁用对[趋势](/graph/api/resources/insights-trending?view=graph-rest-1.0)API 的代理访问，并禁用用户对 Office Delve 中的文档的访问权限。 设置为 true 还会影响 Office 365 中显示的内容的相关性（例如，SharePoint 主页中的建议网站和 OneDrive for Business 中的发现视图）显示较少的相关结果。 此设置反映了[Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)中的控件状态。|

## <a name="example"></a>示例 

##### <a name="request"></a>请求

下面的示例请求展示了如何从 Delve 中选择用户，并对整个组织禁用其对内容相关性的贡献。

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```



