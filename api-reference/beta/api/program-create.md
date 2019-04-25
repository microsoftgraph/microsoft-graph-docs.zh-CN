---
title: 创建程序
description: 在 "Azure AD access 评论" 功能中, 创建一个新的程序对象。
localization_priority: Normal
ms.openlocfilehash: a6e9ab300cf44a2f3973c468679af7fa48262680
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538537"
---
# <a name="create-program"></a>创建程序

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 创建一个新的[程序](../resources/program.md)对象。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | `ProgramControl.ReadWrite.All`.  登录用户还必须位于允许他们创建程序的目录角色中。 |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中, 提供[程序](../resources/program.md)对象的 JSON 表示形式。

下表显示创建程序时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  程序的名称。                   |
| `description`               |`String`                              |  程序的说明。           |


## <a name="response"></a>响应
如果成功, 此方法在响应`201, Created`正文中返回响应代码和[程序](../resources/program.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
在请求正文中, 提供[程序](../resources/program.md)对象的 JSON 表示形式。

<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
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
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出程序](program-list.md) | [程序](../resources/program.md)集|  获取所有程序的集合。|
|[列出程序的 programControls](program-listcontrols.md) |     [programControl](../resources/programcontrol.md)集合|    获取程序的控件的集合。|
|[更新程序](program-update.md) |  [主程序](../resources/program.md)| 更新程序。|
|[创建 programControl](programcontrol-create.md) |        [programControl](../resources/programcontrol.md)    |   将 programControl 添加到程序中。|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
