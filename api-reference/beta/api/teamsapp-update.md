---
title: 权限
description: '更新之前发布到 Microsoft 团队应用程序目录的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 02822690d18076ee5ce2535c06e2856afe89e3c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977547"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a>更新发布到组织的应用程序目录的应用程序

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新之前发布到 Microsoft 团队应用程序目录的[应用程序](../resources/teamsapp.md)。 此 API 专门更新发布到您的组织的应用程序目录 (租户应用程序目录) 的应用程序。 若要发布到您的组织的应用程序`organization`目录, 请在[teamsCatalogApp](../resources/teamsapp.md)资源中将其指定为**distributionMethod** 。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。

>**注意:** 只有全局管理员才能调用此 API。

| 权限类型                        | 权限（从最低特权到最高特权）|
|:----------------------------------     |:-------------|
| 委派（工作或学校帐户）     | AppCatalog.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持|
| 应用程序                            | 不支持|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a>请求标头

| 标头        | 值           |
|:--------------|:--------------  |
| Authorization | Bearer {token}。必需。  |
| Content-Type  | application/zip |

## <a name="request-body"></a>请求正文

团队 Zip 清单有效负载: 对于团队应用程序 Zip 文件,[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

>**注意:** 使用从[列表已发布的应用程序](./teamsapp-list.md)调用中返回的 ID 引用要更新的应用程序。 请勿使用 zip 应用程序包清单中的 ID。

## <a name="response"></a>响应

```
HTTP/1.1 204 No Content
```

## <a name="example"></a>示例

### <a name="request"></a>请求

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

对于团队应用程序 zip 文件,[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

### <a name="response"></a>响应

```
HTTP/1.1 204 No Content
```
