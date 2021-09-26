---
title: 删除 organizationalBranding
description: 删除 organizationalBranding 对象。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4ce769c52af786bbd7893e4cac1832c19ce87391
ms.sourcegitcommit: 7ce66321abb6a2cdca8685d3ce0a004c376ae33b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777987"
---
# <a name="delete-organizationalbranding"></a>删除 organizationalBranding
命名空间：microsoft.graph

删除默认组织品牌对象。 若要删除 [organizationalBranding](../resources/organizationalbranding.md) 对象，必须先 (对象) Stream 类型的所有图像。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Organization.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /organization/{organizationId}/branding
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

在请求正文中，提供默认 [organizationalBranding 对象的](../resources/organizationalbranding.md) JSON 表示形式。 仅 **id** 属性是必需的。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "delete_organizationalbranding"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding

{
    "id": "0"
}
```


### <a name="response"></a>响应

下面展示了示例响应。
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

