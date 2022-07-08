---
title: 列出 teamTemplates
description: 获取 teamTemplate 对象及其租户属性的列表。
author: Charlieforce
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: ce9261b636a0d5f53b3c92d9795624b9b1ddd931
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690112"
---
# <a name="list-teamtemplates"></a>列出 teamTemplates
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取可用于租户的 [teamTemplate](../resources/teamtemplate.md) 对象的列表。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Team.Create|
|委派（个人 Microsoft 帐户）|不支持|
|Application|Team.Create|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/teamTemplates
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$expand``$filter``$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法将返回 `200 OK` 响应代码和 [teamTemplate](../resources/teamtemplate.md) 对象的集合。 

> [!Note]
> 目前，此 API 仅返回 [teamTemplate](../resources/teamtemplate.md) 的 **ID** 属性。 若要获取 [teamTemplateDefinition](../resources/teamtemplatedefinition.md)，请使用 OData 查询参数 `$expand=definitions`。

## <a name="examples"></a>示例

## <a name="example-1-get-a-list-of-team-templates"></a>示例 1：获取团队模板列表

### <a name="request"></a>请求
请求示例如下所示。


<!-- {
  "blockType": "request",
  "name": "list_teamtemplatedefinition"
}
-->
```http 
GET https://graph.microsoft.com/beta/teamwork/teamTemplates
```

### <a name="response"></a>响应
下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamtemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "id": "com.microsoft.teams.template.ManageAProject"
        },
        {
            "id": "com.microsoft.teams.template.ManageAnEvent"
        }
    ]
}
```

### <a name="example-2-use-extend-and-filter-to-get-templatedefinitions-for-en-us-locale"></a>示例 2：使用$extend和$filter获取 en-US 区域设置的模板Definitions

### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "list_teamtemplatedefinition"
}
-->
```http
GET https://graph.microsoft.com/beta/teamwork/teamTemplates?$expand=definitions&filter=definitions/any(a:a/languageTag eq 'en-US')
```

### <a name="response"></a>响应
下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamtemplatedefinition)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "id": "com.microsoft.teams.template.ManageAProject",
            "definitions": [
                {
                    "id": "Y29tLm1pY3Jvc29mdC50ZWFtcy50ZW1wbGF0ZS5NYW5hZ2VBUHJvamVjdCMjUHVibGljIyNlbi1VUw==",
                    "parentTemplateId": "com.microsoft.teams.template.ManageAProject",
                    "displayName": "Manage a Project",
                    "languageTag": "en-US",
                    "audience": "public",
                    "description": "Manage tasks, share documents, conduct project meetings and document risks and decisions with this template for general project management.",
                    "shortDescription": "Coordinate your project.",
                    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
                    "publisherName": "Microsoft",
                    "categories": [
                        "General"
                    ],
                    "lastModifiedBy": null
                }
            ]
        },
        {
            "id": "com.microsoft.teams.template.ManageAnEvent",
            "definitions": [
                {
                    "id": "Y29tLm1pY3Jvc29mdC50ZWFtcy50ZW1wbGF0ZS5NYW5hZ2VBbkV2ZW50IyNQdWJsaWMjI2VuLVVT",
                    "parentTemplateId": "com.microsoft.teams.template.ManageAnEvent",
                    "displayName": "Manage an Event",
                    "languageTag": "en-US",
                    "audience": "public",
                    "description": "Manage tasks, documents, and collaborate on everything you need to deliver a compelling event. Invite guest users to have a secure collaboration inside and outside of your company.",
                    "shortDescription": "Improve your event management and collaboration.",
                    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
                    "publisherName": "Microsoft",
                    "categories": [
                        "General"
                    ],
                    "lastModifiedBy": null
                }
            ]
        },
    ]
}
```
