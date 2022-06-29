---
title: 创建 retentionEventType
description: 创建新的 retentionEventType 对象。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 986615de931ba4c08e78880776079ac4ab9c6ce0
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447547"
---
# <a name="create-retentioneventtype"></a>创建 retentionEventType
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [retentionEventType](../resources/security-retentioneventtype.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RecordsManagement.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|RecordsManagement.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/triggerTypes/retentionEventTypes
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [retentionEventType](../resources/security-retentioneventtype.md) 对象的 JSON 表示形式。

创建 **retentionEventType** 时指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|事件类型的名称。|
|说明|String|有关事件类型的信息。 可选。|




## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_retentioneventtype_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/triggerTypes/retentionEventTypes
Content-Type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.security.retentionEventType",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.retentionEventType"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.security.retentionEventType",
  "id": "dd689e79-9e79-dd68-799e-68dd799e68dd",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

