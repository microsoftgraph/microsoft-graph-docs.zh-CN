---
title: 获取 contactMergeSuggestions
description: 读取 contactMergeSuggestions 对象的属性和关系。
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 108e6b724885507d8d51e0b5049b1dc4e68d98c1
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338292"
---
# <a name="get-contactmergesuggestions"></a>获取 contactMergeSuggestions
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [contactMergeSuggestions](../resources/contactmergesuggestions.md) 对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|User.Read、User.ReadWrite|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/settings/contactMergeSuggestions
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [contactMergeSuggestions](../resources/contactmergesuggestions.md) 对象。

## <a name="examples"></a>示例

下面是请求获取用户的 **contactMergeSuggestions** 设置的示例。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_contactmergesuggestions"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/settings/contactMergeSuggestions
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactMergeSuggestions",
  "name": "get_contactmergesuggestions"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "isEnabled": true
}
```

