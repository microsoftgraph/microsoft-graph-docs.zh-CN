---
title: 创建 programControl
description: 在 Azure AD 访问评审功能中，创建新的 programControl 对象。  这会将访问评审链接到计划。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 4d70ea6dacb12b56a4ae14486cb0ed5adcb6850b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442201"
---
# <a name="create-programcontrol"></a>创建 programControl

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，创建新的 [programControl](../resources/programcontrol.md) 对象。  这会将访问评审链接到计划。

在提出此请求之前，呼叫者必须事先拥有

- [创建程序](program-create.md) 或 [检索程序](program-list.md)，以将值 `programId` 包括在请求中，
- [创建访问评审](accessreview-create.md) 或 [检索访问评审](accessreview-get.md)，以将值包括在请求 `controlId` 中，
- [检索程序控件类型列表](programcontroltype-list.md)，以将值 `controlTypeId` 包括在请求中。


## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | ProgramControl.ReadWrite.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application                            |  ProgramControl.ReadWrite.All  |

登录用户还必须在允许他们创建 **programControl** 的目录角色中。 

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
在请求正文中，提供 [programControl](../resources/programcontrol.md) 对象的 JSON 表示形式。

下表显示创建程序控件时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| `programId`              |`String`                | 此控件将成为其一部分的程序的 programId。                             |
| `controlId`              |`String`                | 控件的 controlId，尤其是访问评审的标识符。                                                |
| `controlTypeId`          |`String`                | programControlType 标识程序控件的类型-例如，链接到来宾访问评审的控件。 |

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回响应 `201, Created` 代码和 [programControl](../resources/programcontrol.md) 对象。


## <a name="example"></a>示例
##### <a name="request"></a>请求
在请求正文中，提供 [programControl](../resources/programcontrol.md) 对象的 JSON 表示形式。


# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-programcontrol-from-programcontrols-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-programcontrol-from-programcontrols-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-programcontrol-from-programcontrols-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-programcontrol-from-programcontrols-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
|[列出 programControlTypes](../api/programcontroltype-list.md) | [programControlType](../resources/programcontroltype.md) 集合| 列出程序控件类型。 |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


