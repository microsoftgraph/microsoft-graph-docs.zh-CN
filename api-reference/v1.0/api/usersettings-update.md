---
title: 更新设置
description: '更新 settings 对象的属性。 '
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: eac479222b271e6143fb8e3f8b46b5bfa9aadce1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897489"
---
# <a name="update-settings"></a>更新设置

命名空间：microsoft.graph

更新[userSettings](../resources/usersettings.md)对象的属性。 同一个组织中的用户可以根据自己的首选项或组织策略拥有不同的设置。 若要获取用户的当前设置，请参阅[当前用户设置](usersettings-get.md)。 

### <a name="batch-request"></a>批量请求

此外，还可以从 Delve 中自愿退出多个用户，并通过批处理请求禁用对整个组织的内容关联的贡献。
若要了解详细信息，请参阅[JSON 批处理](https://developer.microsoft.com/graph/docs/concepts/json_batching)。

>**重要说明**：只有[组织管理](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US)角色组的成员才能更新多个用户。 



## <a name="permissions"></a>权限

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

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
| Authorization  | Bearer {token}. Required.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文

In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|布尔值|设置为 true 确实禁用对[趋势](/graph/api/resources/insights-trending?view=graph-rest-1.0)API 的代理访问，并禁用用户对 Office Delve 中的文档的访问权限。 设置为 true 还会影响 Microsoft 365 中显示的内容的相关性（例如，SharePoint 主页中的建议网站和 OneDrive for Business 中的发现视图）显示较少的相关结果。 此设置反映了[Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)中的控件状态。|

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

Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```



