---
title: 列出 privilegedOperationEvents
description: 筛选器 ' ' 表达式。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: e0fc6347b273a046b202aecd803434d0f6fa0af8
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218778"
---
# <a name="list-privilegedoperationevents"></a>列出 privilegedOperationEvents

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索[privilegedOperationEvent](../resources/privilegedoperationevent.md)对象的列表，这些对象表示由角色操作的特权标识管理生成的审核事件。 有关审核事件的详细信息，请参阅[privilegedOperationEvent](../resources/privilegedoperationevent.md)。 若要筛选查询结果，请使用标准 OData ``$filter``表达式。


## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

请求者需要具有以下角色之一：_特权角色管理员_、_全局管理员_、_安全管理员_或_安全读者_。

 

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedOperationEvents
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和[privilegedOperationEvent](../resources/privilegedoperationevent.md)对象集合。

请注意，需要将租户注册到 PIM。 否则，将返回 HTTP 403 禁止的状态代码。
## <a name="examples"></a>示例

### <a name="get-audit-events-for-role-assignment-operations"></a>获取角色分配操作的审核事件
##### <a name="request"></a>请求
以下示例显示了获取角色分配操作的审核事件的请求。 在这种情况``requestType``下， ``Assign``value 为。

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=requestType%20eq%20'Assign'
```
##### <a name="response"></a>响应
以下示例显示了相应的响应。 注意：为简洁起见，可能会截断此处显示的响应对象。 所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "value": [
        {
            "id": "201707240003469369",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f80",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "9360feb5-f418-4baa-8175-e2a00bac4301",
            "roleName": "Directory Writers",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T18:32:38.7589078Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Assign",
            "additionalInformation": null,
            "referenceKey": null,
            "referenceSystem": null
        },
        {
            "id": "201707240003469372",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f80",
            "userName": "admin",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T18:33:00.7607701Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Assign",
            "additionalInformation": null,
            "referenceKey": null,
            "referenceSystem": null
        }
    ]
}
```
### <a name="get-audit-events-for-the-operations-of-self-role-activation-and-makepermanent"></a>获取自我角色激活和 makePermanent 操作的审核事件
##### <a name="request"></a>请求
下面的示例演示获取获取自我角色激活和 makePermanent 操作的审核事件的请求。 在这种情况``requestType``下， ``Activate``value 为。

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=requestType%20eq%20'Activate'
```
##### <a name="response"></a>响应
以下示例显示了相应的响应。 注意：为简洁起见，可能会截断此处显示的响应对象。 所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "value": [
        {
            "id": "201707240003469811",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "44367163-eba1-44c3-98af-f5787879f96a",
            "roleName": "CRM Service Administrator",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T23:34:41.9661094Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin1",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Activate",
            "additionalInformation": "Make permanent admin",
            "referenceKey": null,
            "referenceSystem": null
        },
        {
            "id": "201707240003469814",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "2017-07-25T00:37:07.3402169Z",
            "creationDateTime": "2017-07-24T23:37:08.0052112Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin1",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Activate",
            "additionalInformation": "self activate",
            "referenceKey": "",
            "referenceSystem": ""
        }
    ]
}
```

### <a name="get-audit-events-for-role-assignment-deactivation"></a>获取角色分配停用的审核事件
##### <a name="request"></a>请求
下面的示例演示获取获取角色分配停用的审核事件的请求。 在这种情况``requestType``下， ``Deactivate``value 为。

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=requestType%20eq%20'Deactivate'
```
##### <a name="response"></a>响应
以下示例显示了相应的响应。 注意：为简洁起见，可能会截断此处显示的响应对象。 所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "value": [
        {
            "id": "201707240003469375",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f80",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T18:33:28.3408971Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin1",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Deactivate",
            "additionalInformation": "Make eligible admin",
            "referenceKey": null,
            "referenceSystem": null
        }
    ]
}
```
### <a name="get-audit-events-created-in-a-time-range"></a>获取在某个时间范围内创建的审核事件
##### <a name="request"></a>请求 
下面的示例展示了获取在某个时间范围内创建的审核事件的请求。

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=(creationDateTime%20ge%202017-06-25T07:00:00Z)%20and%20(creationDateTime%20le%202017-07-25T17:30:17Z)&$count=true&$orderby=creationDateTime%20desc
```
##### <a name="response"></a>响应
以下示例显示了相应的响应。 注意：为简洁起见，可能会截断此处显示的响应对象。 将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedOperationEvents",
    "@odata.count": 2,
    "value": [
        {
            "id": "201707250003471056",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin",
            "userMail": "admin@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "2017-07-25T17:38:49.5640383Z",
            "creationDateTime": "2017-07-25T16:38:50.3681771Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Activate",
            "additionalInformation": "activate test",
            "referenceKey": "",
            "referenceSystem": ""
        },
        {
            "id": "201707250003469896",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin",
            "userMail": "admin@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-25T00:37:08.6172407Z",
            "requestorId": "6b61baec-bb80-4a8a-b8bd-fa5ba1f12386",
            "requestorName": "Azure AD PIM",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Deactivate",
            "additionalInformation": "Expired",
            "referenceKey": "",
            "referenceSystem": ""
        }
    ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedOperationEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
