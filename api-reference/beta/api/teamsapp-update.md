---
title: 更新 teamsApp
description: '更新之前发布到 Microsoft 团队应用程序目录的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b5de60708ec0c8a6a0e22cd4f64b847395620bd0
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806316"
---
# <a name="update-teamsapp"></a>更新 teamsApp

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新之前发布到 Microsoft 团队应用程序目录的 [应用程序](../resources/teamsapp.md) 。 若要更新应用程序，必须将应用程序的 **distributionMethod** 属性设置为 `organization` 。

此 API 专门更新 (租户应用程序目录) 发布到组织的应用程序目录中的应用程序。  

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。

>**注意：** 只有全局管理员才能调用此 API。

| 权限类型                        | 权限（从最低特权到最高特权）|
|:----------------------------------     |:-------------|
| 委派（工作或学校帐户）     | AppCatalog、所有的目录读写。 |
| 委派（工作或学校帐户） | AppCatalog.Submit|
| 委派（个人 Microsoft 帐户） | 不支持|
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a>查询参数

|属性|类型|说明|
|----|----|----|
|requiresReview| 布尔值 | 此可选查询参数触发应用程序审阅过程。 具有管理员权限的用户无需触发评审即可提交应用程序。 如果用户希望在发布之前请求审阅，则必须将其设置  `requiresReview` 为 `true` 。 具有管理员权限的用户可以选择不设置 `requiresReview` 或设置值 `false`  ，并且应用将被视为 "已批准"，并将立即发布。|

## <a name="request-headers"></a>请求标头

| 标头        | 值           |
|:--------------|:--------------  |
| Authorization | Bearer {token}。必需。  |
| Content-Type  | application/zip。 必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，包括团队 zip 清单有效负载。 有关详细信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。

>**注意：** 使用从 [列表已发布的应用程序](./teamsapp-list.md) 调用中返回的 ID 引用要更新的应用程序。 请勿使用 zip 应用程序包清单中的 ID。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a>示例1：更新之前发布到 Microsoft 团队应用程序目录的应用程序

### <a name="request"></a>请求

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8/appDefinitions
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

有关团队应用程序 zip 文件的详细信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。
<!-- markdownlint-disable MD024 -->

### <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

### <a name="example-2-update-a-new-version-of-an-existing-app-for-admin-review-prior-to-publication-in-the-current-tenant-catalog"></a>示例2：在当前租户目录中发布之前更新现有应用程序的新版本，以供管理员审阅

### <a name="request"></a>请求

<!-- markdownlint-disable MD034 -->

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions?requiresReview=true
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

如果成功，此方法 `201 Created` `publishingState` `submitted` 在响应正文中返回响应代码和键/值对：。 *请参阅* [teamsappdefinition](../resources/teamsappdefinition.md)。

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions/MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appDefinition",
    "@odata.etag": "158749010",
    "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
    "teamsAppId": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
    "displayName": "Test app",
    "version": "1.0.11",
    "azureADAppId": "a651cc7d-ec54-4fb2-9d0e-2c58dc830b0b",
    "requiredResourceSpecificApplicationPermissions":[
         "ChannelMessage.Read.Group",
         "Channel.Create.Group",
         "Tab.ReadWrite.Group",
         "Member.Read.Group"
    ],
    "publishingState": "submitted",
    "lastModifiedDateTime": "2020-02-10 22:48:33.841",
}
```
