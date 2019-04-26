---
title: '部分: copyToSectionGroup'
description: 将分区复制到特定分区组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 3e0968ec4ecae4cd8eaff0ff257e5e87220e7fc9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336093"
---
# <a name="section-copytosectiongroup"></a>部分: copyToSectionGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将分区复制到特定分区组。

对于复制操作, 请遵循异步调用模式: 首先调用复制操作, 然后轮询操作终结点以获取结果。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Notes.Create、Notes.ReadWrite    |
|应用程序 | Notes.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type | string | `application/json` |

## <a name="request-body"></a>请求正文
在请求正文中, 提供一个 JSON 对象, 其中包含您的操作所需的参数。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|siteCollectionId|String|要复制到的 SharePoint 网站的 id。 仅在复制到 Office 365 团队网站时使用。|
|siteId|String|要复制到的 SharePoint 网站的 id。 仅在复制到 Office 365 团队网站时使用。|
|groupId|String|要复制到的组的 id。 仅在复制到 Office 365 组时使用。|
|id|String|必需。 目标分区组的 id。 |
|renameAs|String|副本的名称。 默认值为现有项目的名称。 |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a>响应

如果成功, 此方法将`202 Accepted`返回响应代码和`Operation-Location`标头。 轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
