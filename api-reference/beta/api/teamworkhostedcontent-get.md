---
title: 获取 teamworkHostedContent
description: 检索 teamsAppIcon 中的托管内容。
localization_priority: Normal
author: jecha
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1b5fde96ffaad34360603751398473357d82e1fd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882648"
---
# <a name="get-teamworkhostedcontent"></a>获取 teamworkHostedContent

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [应用的图标](../resources/teamworkhostedcontent.md) 中检索 [托管的内容](../resources/teamsappicon.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="permissions-for-app-icon-in-app-catalog"></a>应用程序目录中应用程序图标的权限
| 权限类型                        | 权限（从最低特权到最高特权）                      |
| :------------------------------------- | :--------------------------------------------------------------- |
| 委派（工作或学校帐户）     | AppCatalog.Read.All、AppCatalog.ReadWrite.All、AppCatalog.Submit |
| 委派（个人 Microsoft 帐户） | 不支持。                                                   |
| 应用程序                            | 不支持。                                                   |

## <a name="http-request"></a>HTTP 请求

**获取应用程序目录中应用程序图标中的托管内容**

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/$value
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/$value
```

## <a name="optional-query-parameters"></a>可选的查询参数

此操作支持使用 `$select` [OData 查询参数](/graph/query-parameter) 自定义响应。

## <a name="request-headers"></a>请求标头

| 标头           | 值                      |
| :--------------- | :------------------------- |
| Authorization    | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [teamworkHostedContent](../resources/teamworkhostedcontent.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-get-the-bytes-of-the-hosted-content-of-the-color-icon-of-a-teams-app-in-the-catalog"></a>示例 1：获取目录中 Teams 应用的颜色图标的托管内容的字节数

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontent_coloricon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon/hostedContent/
```


#### <a name="response"></a>响应

以下示例显示了相应的响应。

> **注意：** `contentBytes` 和 `contentType` 始终设置为 null。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/colorIcon/hostedContent/$entity",
    "id": "aWQ9LHR5cGU9MSx1cmw9aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWQwOGVkNTQ2MjQ2MTliNTc4OGIwMWUzODNlMWVjYzU3L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-the-bytes-of-the-hosted-content-of-the-outline-icon-of-a-teams-app-in-the-catalog"></a>示例 2：获取目录中 Teams 应用的大纲图标的托管内容的字节数

#### <a name="request"></a>请求

下面展示了示例请求。

> **注意：** 对原始值的请求不支持 [使用 OData 查询参数](/graph/query-parameters) 自定义响应。

<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontentbytes_outlineicon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon/hostedContent/$value
```

#### <a name="response"></a>响应

响应包含正文中托管内容的字节。 `content-type` header 指定托管内容类型。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: image/png
```

## <a name="see-also"></a>另请参阅

- [获取 Teams 应用的图标](teamsappicon-get.md)
- [列出目录中的应用](appcatalogs-list-teamsapps.md)
