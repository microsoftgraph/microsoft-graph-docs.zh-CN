---
title: 创建团队合作标记
description: 创建新的团队合作标记对象。
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b379037f01b5d28c867de0083ec6f7a581f0ea80
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060659"
---
# <a name="create-teamworktag"></a>创建团队合作标记
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为团队 [中的成员](../resources/teamworktag.md) 创建标准标记。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|不支持。|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|TeamworkTag.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{team-Id}/tags
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [teamworkTag](../resources/teamworktag.md) 对象的 JSON 表示形式。

下表显示创建团队合作标记 时所需的 [属性](../resources/teamworktag.md)。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|标记的名称。 该值不能超过 40 个字符。|
|members| [teamworkTagMember](../resources/teamworktagmember.md) 集合 |要添加到标记的团队成员。 设置每个成员的用户标识符属性。 成员计数不应超过 25。|



## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [团队合作](../resources/teamworktag.md) Tag 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_teamworktag_from"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags
Content-Type: application/json

{
  "displayName": "Finance",
  "members":[
    {
        "userId":"92f6952f-61ca-4a94-8910-508a240bc167"
    },
    {
        "userId":"085d800c-b86b-4bfc-a857-9371ad1caf29"
    }
  ]
}
```


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
  "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
  "displayName": "Financee",
  "memberCount": 2,
  "tagType": "standard"
}
```

