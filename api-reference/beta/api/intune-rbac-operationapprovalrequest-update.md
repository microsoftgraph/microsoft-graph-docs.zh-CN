---
title: Update operationApprovalRequest
description: 更新 operationApprovalRequest 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ce96e13b791db9667cc1ea07fb3ee1d21182410
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60485040"
---
# <a name="update-operationapprovalrequest"></a>Update operationApprovalRequest

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [operationApprovalRequest 对象](../resources/intune-rbac-operationapprovalrequest.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementRBAC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/operationApprovalRequests/{operationApprovalRequestId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) 对象的 JSON 表示形式。

下表显示创建 [operationApprovalRequest 时所需的属性](../resources/intune-rbac-operationapprovalrequest.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的 ID|
|requestDateTime|DateTimeOffset|请求的 DateTime。 此属性是只读的。|
|expirationDateTime|DateTimeOffset|不再允许对请求执行操作的日期/时间。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|上次修改日期时间。 此属性是只读的。|
|requestor|[identitySet](../resources/intune-rbac-identityset.md)|请求者的身份。 此属性是只读的。|
|审批者|[identitySet](../resources/intune-rbac-identityset.md)|审批者的身份。 此属性是只读的。|
|status|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|当前审批请求状态。 此属性是只读的。 可取值为：`unknown`、`needsApproval`、`approved`、`rejected`、`cancelled`、`completed` 或 `expired`。|
|requestJustification|String|请求理由。 此属性是只读的。|
|approvalJustification|String|批准请求的理由。 此属性是只读的。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/operationApprovalRequests/{operationApprovalRequestId}
Content-type: application/json
Content-length: 1346

{
  "@odata.type": "#microsoft.graph.operationApprovalRequest",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "requestor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "approver": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "status": "needsApproval",
  "requestJustification": "Request Justification value",
  "approvalJustification": "Approval Justification value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1459

{
  "@odata.type": "#microsoft.graph.operationApprovalRequest",
  "id": "4e9eed82-ed82-4e9e-82ed-9e4e82ed9e4e",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "requestor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "approver": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "status": "needsApproval",
  "requestJustification": "Request Justification value",
  "approvalJustification": "Approval Justification value"
}
```



