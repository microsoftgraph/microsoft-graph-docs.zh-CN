---
title: 创建 programControl
description: Azure AD 中访问审阅功能，创建一个新的 programControl 对象。  这会链接到程序访问审阅。
ms.openlocfilehash: fa6a93b13391fd4b9e3c5816bb2a27259e730c0d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047032"
---
# <a name="create-programcontrol"></a>创建 programControl

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中创建新的[programControl](../resources/programcontrol.md)对象。  这会链接到程序访问审阅。

进行此请求之前, 将呼叫者必须具有之前

 - [创建一个程序](program-create.md)或[检索程序](program-list.md)，以使数值`programId`要包含在请求中，
 - [创建访问审阅](accessreview-create.md)或[检索访问审阅](accessreview-get.md)，具有的值`controlId`要包含在请求中，和
 - [检索的程序控件类型的列表](programcontroltype-list.md)，以使数值`controlTypeId`要包含在请求中。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | `ProgramControl.ReadWrite.All`.  登录的用户必须同时是允许他们创建 programControl 目录角色中。 |
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
| Authorization | string | 持有者\{标记\}。 必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供[programControl](../resources/programcontrol.md)对象的 JSON 表示形式。

下表显示时创建一个程序控件所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| `programId`              |`String`                | 程序 programId 此控件将变得的一部分。                             |
| `controlId`              |`String`                | 控件的 controlId，尤其要指出的访问的标识符查看。                                                |
| `controlTypeId`          |`String`                | ProgramControlType 标识的程序控件的类型-例如，将链接到来宾访问控制审阅。 |

## <a name="response"></a>响应
如果成功，此方法返回`201, Created`响应代码和响应正文中的[programControl](../resources/programcontrol.md)对象。


## <a name="example"></a>示例
##### <a name="request"></a>请求
在请求正文中，提供[programControl](../resources/programcontrol.md)对象的 JSON 表示形式。

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
|[列表 programControlTypes](../api/programcontroltype-list.md) | [programControlType](../resources/programcontroltype.md)集合| 列出程序控件类型。 |


<!-- {
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
