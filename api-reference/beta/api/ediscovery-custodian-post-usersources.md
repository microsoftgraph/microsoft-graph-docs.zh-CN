---
title: 创建保管人 userSource
description: 创建新的保管人 userSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 040c4178a269998117e55e86016a4683c5293a2e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446055"
---
# <a name="create-custodian-usersource"></a>创建保管人 userSource

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的保管人 [userSource](../resources/ediscovery-usersource.md) 对象。

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
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/userSources
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [userSource](../resources/ediscovery-usersource.md) 对象的 JSON 表示形式。

下表显示创建 [userSource](../resources/ediscovery-usersource.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|email|String|用户的 SMTP 地址。|
|includedSources|microsoft.graph.ediscovery.sourceType|指定此组中包含的源。 可取值为：`mailbox`、`site`。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和 `201 Created` [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_usersource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources
Content-Type: application/json
Content-length: 233

{
    "email":"megan@contoso.com",
    "includedSources":"mailbox, site"
}
```

---

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.userSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('45454331323337443946343043464239')/userSources/$entity",
    "displayName": "Megan Bowen",
    "createdDateTime": "2020-11-06T16:09:08.4905571Z",
    "id": "34383036-3741-4545-3242-373530353435",
    "email": "megan@contoso.com",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null
        }
    }
}
```
