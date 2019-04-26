---
title: 更新程序
description: 在 "Azure AD access 评论" 功能中, 更新现有的程序对象。
localization_priority: Normal
ms.openlocfilehash: 1097ae014537f285238a9ca7f7f231513aa578e0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337157"
---
# <a name="update-program"></a>更新程序

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 更新现有的[程序](../resources/program.md)对象。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | ProgramControl   |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

登录用户还必须位于允许他们更新程序的目录角色中。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中, 提供[程序](../resources/program.md)对象的 JSON 表示形式。

下表显示了在更新程序时可以提供的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  程序的名称。                   |
| `description`               |`String`                              |  程序的说明。           |


## <a name="response"></a>响应
如果成功, 此方法在响应`204, Accepted`正文中返回响应代码和[程序](../resources/program.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
在请求正文中, 提供要更改的[program](../resources/program.md)对象参数的 JSON 表示形式。

<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```

##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3 new name",
    "description": "test description"
}
```

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出程序的 programControls](program-listcontrols.md) |     [programControl](../resources/programcontrol.md)集合|    获取程序的控件的集合。|
|[创建 programControl](programcontrol-create.md) |        [programControl](../resources/programcontrol.md)    |   将 programControl 添加到程序中。|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
