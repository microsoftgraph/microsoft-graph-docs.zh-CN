---
title: 创建 ediscoveryReviewTag
description: 创建新的 ediscoveryReviewTag 对象。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 126e2b8307fff7749ee28f06744def3de26466f3
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945405"
---
# <a name="create-ediscoveryreviewtag"></a>创建 ediscoveryReviewTag
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 ediscoveryReviewTag 对象。

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/tags
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 对象的 JSON 表示形式。

创建 **ediscoveryReviewTag** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|标记的显示名称。 必需。|
|description|String|标记的说明。 可选。|
|childSelectability|字符串|此值控制 UX 是将标记显示为复选框还是单选按钮组。 可能的值为： `One`. `Many` 必需。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 对象。

## <a name="examples"></a>示例

### <a name="create-a-tag"></a>创建标记
#### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "create_ediscoveryreviewtag_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags

{
    "displayName": "My tag API",
    "description": "Use Graph API to create tags",
    "childSelectability": "Many"
}
```


#### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryReviewTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/tags/$entity",
    "displayName": "My tag API",
    "description": "Use Graph API to create tags",
    "lastModifiedDateTime": "2022-05-23T19:58:26.1573076Z",
    "childSelectability": "Many",
    "id": "7c6cc351-fb90-431f-8562-1b607a3144a4",
    "createdBy": {
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": "MOD Administrator",
            "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
        },
        "application": {
            "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "displayName": "Graph Explorer"
        }
    }
}
```

### <a name="create-a-tag-with-a-parent"></a>使用父级创建标记
#### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "create_ediscoveryreviewtag_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags

{
    "displayName": "My tag API",
    "description": "Use Graph API to create tags",
    "childSelectability": "Many",
    "parent@odata.bind":""
}
```


#### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryReviewTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/tags/$entity",
    "displayName": "My tag API",
    "description": "Use Graph API to create tags",
    "lastModifiedDateTime": "2022-05-23T19:58:26.1573076Z",
    "childSelectability": "Many",
    "id": "7c6cc351-fb90-431f-8562-1b607a3144a4",
    "createdBy": {
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": "MOD Administrator",
            "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
        },
        "application": {
            "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "displayName": "Graph Explorer"
        }
    }
}
```