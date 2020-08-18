---
title: 发布 teamsapp
description: 将应用程序发布到 Microsoft 团队应用程序目录。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8d520ef254db5284f550cde309936968df67894b
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792728"
---
# <a name="publish-teamsapp"></a>发布 teamsApp

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将 [应用程序](../resources/teamsapp.md) 发布到 Microsoft 团队应用程序目录。
具体而言，此 API 会将应用程序发布到 (租户应用程序目录) 的组织目录中。创建的资源的 **distributionMethod** 属性值为 `organization` 。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。

>**注意：** 只有全局管理员才能调用此 API。

| 权限类型                        | 权限（从最低特权到最高特权）|
|:----------------------------------     |:-------------|
| 委派（工作或学校帐户）     | AppCatalog、所有的目录读写。 |
| 委派（工作或学校帐户） | AppCatalog|
| 委派（个人 Microsoft 帐户） | 不支持|
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps
```

若要发布需要评审的应用程序，请执行以下操作：

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
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

应用程序目录中的每个应用程序都必须有一个唯一的清单 `id` 。

## <a name="response"></a>响应

如果成功，此方法将返回 `200 OK` 响应代码和 [teamsApp](../resources/teamsapp.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-publish-an-app-to-the-app-catalog"></a>示例1：将应用程序发布到应用程序目录
#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

有关如何创建 Microsoft 团队应用程序 zip 文件的信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}

```

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a>示例2：将要审阅的新应用程序上载到组织的应用程序目录

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps/$entity",
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
