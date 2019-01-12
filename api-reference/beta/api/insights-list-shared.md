---
title: 共享列表
description: 返回与用户共享的文件列表中的计算的洞察。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: c40f6ba80a39fb7db3b959bc78f317d86f3de8e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921778"
---
# <a name="list-shared"></a>共享列表

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

返回与用户共享的文件列表中的计算的洞察。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
```http
GET /me/insights/shared
```
请求用户 id 或者 userPrincipalName 才可以访问由用户，而不是任何其他人：
```http
GET /users/<id | userPrincipalName>/insights/shared
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。

您可以使用`$filter`查询参数来筛选共享的项目。 例如，基于类型：

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

请参阅可用的容器类型和[resourceVisualization](../resources/insights-resourcevisualization.md)中可以通过筛选的类型。

您还可以检索特定的用户共享的文件。 例如，通过指定`lastshared/sharedby/address`属性：

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

请参阅[sharingDetail](../resources/insights-sharingdetail.md)复杂类型。


## <a name="request-headers"></a>请求标头
| 标头       |  值|
|:-------------|:------|
| Authorization  | Bearer {token}。必需。|
| Accept  | application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应代码以及响应正文中的[共享](../resources/insights-shared.md)项目的列表。
## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastShared" : { 
                "sharedDateTime" : "sharedDateTime-value",  
                "sharingSubject" : "sharingSubject-value",
                "sharingType" : "sharingType-value", 
                "sharedBy" : { 
                    "displayName" : "displayName-value", 
                    "id": "id-value" 
                }
                "sharingReference" : { 
                    "webUrl" : "webUrl-value",
                    "type: "type-value", 
                    "id": "id-value"
                } 
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
```

### <a name="expanding-resource"></a>展开资源
可以扩展共享洞察引用的资源。
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```
