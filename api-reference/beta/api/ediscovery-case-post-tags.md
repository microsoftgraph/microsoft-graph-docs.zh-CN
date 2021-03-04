---
title: 创建标记
description: 创建新的标记对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ee08824511ffd3f32b78d5c04726686eee4d4dd4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446078"
---
# <a name="create-tag"></a>创建标记

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为指定案例创建新标记。  标记在审阅内容时用于审阅集。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.Read.All、eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/tags
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供标记对象的 JSON [表示形式](../resources/ediscovery-tag.md) 。

下表显示创建标记时所需的 [属性](../resources/ediscovery-tag.md)。

|属性|类型|说明|
|:---|:---|:---|
|childSelectability|[microsoft.graph.ediscovery.childSelectability](../resources/ediscovery-tag.md#childselectability-values)|指示单个或多个子标记是否可以与文档关联。 可取值为：`One`、`Many`。  此值控制 UX 是作为复选框还是单选按钮组显示标记。 必需。|
|displayName|String|标记的显示名称。 必需。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和 `201 Created` [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_tag_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags
Content-Type: application/json
Content-length: 235

{
  "displayName":"Privileged",
  "description":"The document is privileged",
  "parent@odata.bind":"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"
}
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.tag"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/$entity",
    "displayName": "Privileged",
    "description": "The document is privileged",
    "lastModifiedDateTime": "2021-01-12T01:01:09.0419153Z",
    "childSelectability": "One",
    "id": "0825ef81ade74095a3b3154a3c434c3e",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```
