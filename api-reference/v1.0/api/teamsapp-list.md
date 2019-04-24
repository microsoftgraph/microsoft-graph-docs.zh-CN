---
title: 列出 Microsoft 团队应用程序目录中已发布的应用程序
description: '列出 Microsoft 团队应用程序目录中的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 884fd932acddb1352c48e82302a6c345fadf90b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521787"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a>列出 Microsoft 团队应用程序目录中已发布的应用程序

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出 Microsoft 团队应用程序目录中的[应用程序](../resources/teamsapp.md)。
这包括 Microsoft 团队存储区中的应用程序, 以及组织的应用程序目录 (租户应用程序目录) 中的应用程序。 若要仅从组织的应用程序目录中获取应用`Organization`程序, 请在[teamsCatalogApp](../resources/teamsapp.md)资源中将其指定为**distributionMethod** 。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。

> **注意:** 只有全局管理员才能调用此 API。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:------------------------------------|
| 委派（工作或学校帐户）     | AppCatalog.ReadWrite.All            |
| 委派（个人 Microsoft 帐户） | 不支持                       |
| Application                            | 不支持                       |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 标头        | 值                     |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

无。

> **注意:** 您可以对[teamsCatalogApp](../resources/teamsapp.md)对象的任何字段进行筛选, 以缩短结果列表。 您可以使用以下任何筛选器操作: 等于、不等于、和、或, 而不是。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[teamsCatalogApp](../resources/teamsapp.md)对象的列表。

## <a name="examples"></a>示例

### <a name="example-1-list-all-applications"></a>示例 1: 列出所有应用程序

下面的示例列出了特定于您的租户的所有应用程序。

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>响应

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a>示例 2: 列出具有给定 ID 的应用程序

下面的示例列出了具有给定 ID 的应用程序。

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a>响应

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
