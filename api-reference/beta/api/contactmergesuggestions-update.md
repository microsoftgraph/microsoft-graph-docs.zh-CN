---
title: 更新 contactMergeSuggestions
description: 更新 contactMergeSuggestions 对象的属性。
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 582bf04e32f449d4dedd597451bdd14c8676a073
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338385"
---
# <a name="update-contactmergesuggestions"></a>更新 contactMergeSuggestions
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [contactMergeSuggestions 对象](../resources/contactmergesuggestions.md) 的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|User.ReadWrite|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/settings/contactMergeSuggestions
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|isEnabled|Boolean|`true` 如果为用户启用了重复的联系人合并建议功能; `false` 如果禁用此功能。 默认值为“`true`”。|



## <a name="response"></a>响应

如果成功，此方法将返回 响应 `204 No Content` 代码，并且该值在后端更新。

## <a name="examples"></a>示例

以下示例更新 **isEnabled** 隐私设置以禁用重复的联系人合并建议功能。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_contactmergesuggestions"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/settings/contactMergeSuggestions
Content-Type: application/json

{
  "isEnabled": false
}
```


### <a name="response"></a>响应

下面展示了示例响应。 

<!-- {
  "blockType": "response",
  "name": "update_contactmergesuggestions"
}
-->
``` http
HTTP/1.1 204 No Content
```

