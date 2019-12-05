---
title: 使用的列表
description: 计算得出的见解，可返回用户使用的文件列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 8a9a1114b5e247807b952d15901b5def124a245a
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844348"
---
# <a name="list-used"></a>使用的列表

计算的洞察力，包括用户修改的文档列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
获取已登录用户已修改的文档列表：

```http
GET /me/insights/used
```

获取指定用户已修改的文档列表。

>**注意**：请求其他用户的已**使用**文档返回按**lastModifiedDateTime**排序的结果。 然后，将**lastAccessedDateTime**设置为**lastModifiedDateTime**。
```http
GET /users/{id | userPrincipalName}/insights/used
```

扩展**使用**的洞察力引用的资源：

```http
GET /me/insights/used/{id}/resource
GET /users/{id | userPrincipalName}/insights/used/{id}/resource
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。

您可以使用`$filter`查询参数筛选已使用的项目。 例如，基于**类型**：

`https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

或基于**containerType**：

`https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

请参阅可在[resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。


## <a name="request-headers"></a>请求标头
| 标头       |  值|
|:-------------|:------|
| Authorization  | Bearer {token}。必需。|
| 接受  | application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和已[使用](../resources/insights-used.md)项的列表。
## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。
```http
GET https://graph.microsoft.com/v1.0/me/insights/used
```

##### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。 
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastused" : { 
                "lastAccessedDateTime" : "lastAccessedDateTime-value", 
                "lastModifiedDateTime": "lastModifiedDateTime-value" 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
            }
        }
    ]
}
```


