---
title: getMyRequestById 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7edfeca72ccef3d8e914c8c00498fc2b5fb0a70f
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630301"
---
# <a name="getmyrequestbyid-function"></a>getMyRequestById 函数

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/operationApprovalRequests/getMyRequestById
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求 URL 中，提供以下查询参数（含值）。
下表显示了可用于此函数的参数。

|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|



## <a name="response"></a>响应
如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和 [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) 。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/operationApprovalRequests/getMyRequestById(id='parameterValue')
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1637

{
  "value": {
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
    "approvalJustification": "Approval Justification value",
    "operationApprovalPolicies": "Operation Approval Policies value"
  }
}
```




