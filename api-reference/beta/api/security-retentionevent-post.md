---
title: 创建 retentionEvent
description: 创建新的 retentionEvent 对象。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: b445bd8b64333c7ba7222f18c3d60feca0aaf3ee
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447563"
---
# <a name="create-retentionevent"></a>创建 retentionEvent
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [retentionEvent](../resources/security-retentionevent.md) 对象。

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
POST /security/triggers/retentionEvents
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [retentionEvent](../resources/security-retentionevent.md) 对象的 JSON 表示形式。

创建 **retentionEvent** 时指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|说明|String|有关事件的可选信息。|
|displayName|String|事件的名称。|
|eventQueries|[microsoft.graph.security.eventQueries](../resources/security-eventqueries.md) 集合| 表示与保留事件关联的工作负荷 (SharePoint Online、OneDrive for Business、Exchange Online) 和标识信息。|
|eventTriggerDateTime|DateTimeOffset|应触发事件的可选时间。|
|retentionEventType|String|与事件关联的事件类型的名称。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_retentionevent_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/triggers/retentionEvents
Content-Type: application/json
Content-length: 616

{
  "@odata.type": "#microsoft.graph.security.retentionEvent",
  "displayName": "String",
  "description": "String",
  "eventQueries": [
    {
      "@odata.type": "microsoft.graph.security.eventQueries"
    }
  ],
  "eventTriggerDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "eventPropagationResults": [
    {
      "@odata.type": "microsoft.graph.security.eventPropagationResult"
    }
  ],
  "eventStatus": {
    "@odata.type": "microsoft.graph.security.retentionEventStatus"
  },
  "lastStatusUpdateDateTime": "String (timestamp)"
}
```


### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.retentionEvent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.security.retentionEvent",
  "id": "fcdbfb58-d0c6-85dd-d011-4e0ff9a6805d",
  "displayName": "String",
  "description": "String",
  "eventQueries": [
    {
      "@odata.type": "microsoft.graph.security.eventQueries"
    }
  ],
  "eventTriggerDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "eventPropagationResults": [
    {
      "@odata.type": "microsoft.graph.security.eventPropagationResult"
    }
  ],
  "eventStatus": {
    "@odata.type": "microsoft.graph.security.retentionEventStatus"
  },
  "lastStatusUpdateDateTime": "String (timestamp)"
}
```

