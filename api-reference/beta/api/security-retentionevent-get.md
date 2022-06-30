---
title: 获取 retentionEvent
description: 读取 retentionEvent 对象的属性和关系。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: c0d195162607f04d0ab92ecd9dfb83da319649b4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447596"
---
# <a name="get-retentionevent"></a>获取 retentionEvent
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [retentionEvent](../resources/security-retentionevent.md) 对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RecordsManagement.Read.All、RecordsManagement.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|RecordsManagement.Read.All、RecordsManagement.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/triggers/retentionEvents/{retentionEventId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持展开 OData 查询参数，以帮助自定义响应。 例如，若要检索事件类型，请使用 `$expand=retentionEventType`。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_retentionevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/triggers/retentionEvents/{retentionEventId}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.retentionEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```

