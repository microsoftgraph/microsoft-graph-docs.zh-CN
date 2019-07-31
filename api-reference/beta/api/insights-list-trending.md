---
title: 列出趋势
description: 计算的洞察力, 可返回围绕用户的项目趋势分析的列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 2d84e2c4470b17b3073856a73d0b8cb7251ea830
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953057"
---
# <a name="list-trending"></a>列出趋势

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

计算的洞察力, 可返回围绕用户的项目趋势分析的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。

您可以使用`$filter`查询参数筛选趋势项。 例如, 基于类型:

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

或基于容器类型:

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

请参阅可在[resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。


## <a name="request-headers"></a>请求标头
| 标头       |  值|
|:-------------|:------|
| Authorization  | Bearer {token}。必需。|
| 接受  | application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[趋势](../resources/insights-trending.md)项列表。 每个项目都包含可视化属性, 用于显示您的体验中的项目。

## <a name="example"></a>示例
#### <a name="request"></a>请求
下面是一个请求示例。
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a>响应
下面是一个响应示例。 注意：为简洁起见，可能会截断此处显示的响应对象。 将从实际调用中返回所有属性。 请参阅页面底部的 "未截断的示例" 响应。
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 801

{
    "value": [
        {
            "id": "id-value",
            "weight": "weight-value",
            "resourceVisualization": {
                "title": "title-value",
                "type": "type-value",
                "mediaType": "mediaType-value",
                "previewImageUrl": "previewImageUrl-value",
                "previewText": "previewText-value",
                "containerWebUrl": "containerWebUrl-value",
                "containerDisplayName": "containerDisplayName-value",
                "containerType": "containerType-value"
            },
            "resourceReference": {
                "webUrl": "webUrl-value",
                "id": "id-value",
                "type": "type-value"
            }
        }
    ]
}
```

### <a name="expanding-resource"></a>扩展资源
可展开趋势洞察力引用的资源。
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
