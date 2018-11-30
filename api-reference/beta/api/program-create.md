---
title: 创建程序
description: Azure AD 中访问审阅功能，创建一个新的程序对象。
ms.openlocfilehash: 1ac3fa1f0b555fc92449adf0e57217d0a7d50375
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047484"
---
# <a name="create-program"></a>创建程序

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中创建新的[程序](../resources/program.md)对象。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | `ProgramControl.ReadWrite.All`.  登录的用户还必须在目录角色中允许他们创建的程序。 |
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
| Authorization | string | 持有者\{标记\}。 必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供[程序](../resources/program.md)的对象的 JSON 表示形式。

下表显示时创建程序所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  程序的名称。                   |
| `description`               |`String`                              |  该程序的描述。           |


## <a name="response"></a>响应
如果成功，此方法返回`201, Created`响应正文中的响应代码和[程序](../resources/program.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
在请求正文中，提供[程序](../resources/program.md)的对象的 JSON 表示形式。

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
|[列表程序](program-list.md) | [程序](../resources/program.md)集|  获取所有的程序的集合。|
|[对程序的列表 programControls](program-listcontrols.md) |     [programControl](../resources/programcontrol.md)集合|    获取一个程序的控件的集合。|
|[更新程序](program-update.md) |  [程序](../resources/program.md)| 更新程序。|
|[创建 programControl](programcontrol-create.md) |        [programControl](../resources/programcontrol.md)    |   添加到程序 programControl。|

<!-- {
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
