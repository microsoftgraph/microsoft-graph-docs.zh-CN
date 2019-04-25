---
title: 创建 programControl
description: 在 "Azure AD access 评论" 功能中, 创建一个新的 programControl 对象。  这会将访问审核链接到某个程序。
localization_priority: Normal
ms.openlocfilehash: 89e31994ea91dba68e2f4563c64eeab53dd4db93
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546425"
---
# <a name="create-programcontrol"></a>创建 programControl

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 创建一个新的[programControl](../resources/programcontrol.md)对象。  这会将访问审核链接到某个程序。

在发出此请求之前, 呼叫者必须先

 - [创建了一个程序](program-create.md)或[检索了一个程序](program-list.md), 以使`programId`其值包含在请求中,
 - [创建了访问](accessreview-create.md)审核或[检索到访问审核](accessreview-get.md), 以在请求中包含`controlId`的值, 以及
 - [检索了程序控制类型的列表](programcontroltype-list.md), 以将值`controlTypeId`包含在请求中。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | `ProgramControl.ReadWrite.All`.  登录用户还必须位于允许他们创建 programControl 的目录角色中。 |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中, 提供[programControl](../resources/programcontrol.md)对象的 JSON 表示形式。

下表显示创建程序控件时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| `programId`              |`String`                | 此控件将要成为的程序的 programId。                             |
| `controlId`              |`String`                | 控件的 controlId, 特别是 access 评审的标识符。                                                |
| `controlTypeId`          |`String`                | programControlType 标识程序控制的类型-例如, 链接到来宾访问审阅的控件。 |

## <a name="response"></a>响应
如果成功, 此方法在响应`201, Created`正文中返回响应代码和[programControl](../resources/programcontrol.md)对象。


## <a name="example"></a>示例
##### <a name="request"></a>请求
在请求正文中, 提供[programControl](../resources/programcontrol.md)对象的 JSON 表示形式。

<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```

##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 programControlTypes](../api/programcontroltype-list.md) | [programControlType](../resources/programcontroltype.md)集合| 列出程序控制类型。 |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
