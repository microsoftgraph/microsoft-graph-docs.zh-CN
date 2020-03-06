---
title: 权限
description: '从组织的应用程序目录中删除应用程序（租户应用程序目录）。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e6c8e6922836c6a7cccdb0d33befc78f9455e87b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509333"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a>从组织的应用程序目录中删除应用程序

命名空间：microsoft.graph



从组织的应用程序目录中删除[应用程序](../resources/teamsapp.md)（租户应用程序目录）。 若要从组织的应用程序目录中删除应用程序`organization` ，请在[teamsCatalogApp](../resources/teamsapp.md)资源中将其指定为**distributionMethod** 。

## <a name="permissions"></a>权限

需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。

>**注意：** 只有全局管理员才能调用此 API。 

| 权限类型                        | 权限（从最低特权到最高特权）|
|:----------------------------------     |:-------------|
| 委派（工作或学校帐户）     | AppCatalog.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持|
| 应用程序                            | 不支持|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a>请求标头

| 标头        | 值           |
|:--------------|:--------------  |
| Authorization | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

无。

>**注意：** 使用从[列表已发布的应用程序](./teamsapp-list.md)调用中返回的 ID 引用要更新的应用程序。 请勿使用 zip 应用程序包清单中的 ID。

## <a name="response"></a>响应

```
HTTP/1.1 204 No Content
```

## <a name="example"></a>示例

### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a>响应

```http
HTTP/1.1 204 No Content
```
