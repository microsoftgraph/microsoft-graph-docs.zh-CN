---
title: 更新 ediscoveryReviewTag
description: 更新 ediscoveryReviewTag 对象的属性。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a16cbcbe749e5a645779afcfd55c51c804e97f57
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839397"
---
# <a name="update-ediscoveryreviewtag"></a>更新 ediscoveryReviewTag
命名空间：microsoft.graph.security



更新 [ediscoveryReviewTag 对象的](../resources/security-ediscoveryreviewtag.md) 属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.Read.All、eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /security/cases/ediscoveryCases/{ediscoveryCaseId}/tags/{ediscoveryReviewTagId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文



|属性|类型|说明|
|:---|:---|:---|
|displayName|String|标记的显示名称。 必需。|
|description|String|标记的说明。 可选。|
|childSelectability|microsoft.graph.security.childSelectability|此值控制 UX 是将标记显示为复选框还是单选按钮组。 可能的值为： `One`. `Many` 必需。|


## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "update_ediscoveryreviewtag"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags/062de822f17a4a2e9b833aa3f6c37108

{
    "displayName": "My tag API 2",
    "description": "Use Graph API to create tags (updated)"
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

