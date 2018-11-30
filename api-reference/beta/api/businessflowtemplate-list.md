---
title: 列表 businessFlowTemplates
description: 在 Azure AD 中访问审阅功能，列出所有 businessFlowTemplate 对象。
ms.openlocfilehash: 9c6dc976244c60151cb2c230430ab6b4d0dc4b43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042038"
---
# <a name="list-businessflowtemplates"></a>列表 businessFlowTemplates

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，列出所有[businessFlowTemplate](../resources/businessflowtemplate.md)对象。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | `AccessReview.Read.All`, `AccessReview.ReadWrite.All`.  登录的用户还必须在目录角色中允许他们阅读访问审阅。 |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者\{标记\}。 必需。 |

## <a name="request-body"></a>请求正文
应提供没有请求正文。

## <a name="response"></a>响应
如果成功，此方法返回`200, OK`响应代码和响应正文中的[businessFlowTemplate](../resources/businessflowtemplate.md)对象的数组。

## <a name="example"></a>示例
##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessFlowTemplate",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Office 365 Groups' membership"
        } 
    ]
}

```

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 accessReview](accessreview-create.md) |    [accessReview](../resources/accessreview.md) |  创建新 accessReview。 |




<!-- {
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
