---
title: 获取 teamTemplateDefinition
description: 读取 teamTemplateDefinition 对象的属性和关系。
author: Charlieforce
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 775b6f6fd39d549765a5179bc1914abd44fd6ad2
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690113"
---
# <a name="get-teamtemplatedefinition"></a>获取 teamTemplateDefinition
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [teamTemplateDefinition](../resources/teamtemplatedefinition.md) 对象的属性和关系。

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
GET /teamwork/teamTemplates/{teamTemplateId}/definitions/{teamTemplateDefinitionID}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [teamTemplateDefinition](../resources/teamtemplatedefinition.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "get_teamtemplatedefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/teamTemplates/com.microsoft.teams.template.ManageAProject/definitions/Y29tLm1pY3Jvc29mdC50ZWFtcy50ZW1wbGF0ZS5NYW5hZ2VBUHJvamVjdCMjUHVibGljIyNlbi1VUw==
```

### <a name="response"></a>响应
下面是响应的示例

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamtemplatedefinition"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "Y29tLm1pY3Jvc29mdC50ZWFtcy50ZW1wbGF0ZS5NYW5hZ2VBUHJvamVjdCMjUHVibGljIyNlbi1VUw==",
    "parentTemplateId": "com.microsoft.teams.template.ManageAProject",
    "displayName": "Manage a Project",
    "languageTag": "en-US",
    "audience": "public",
    "description": "Manage tasks, share documents, conduct project meetings and document risks and decisions with this template for general project management.",
    "shortDescription": "Coordinate your project.",
    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
    "publisherName": "Microsoft",
    "categories": [],
    "lastModifiedBy": null
  }
}
```
