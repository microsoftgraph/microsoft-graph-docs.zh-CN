---
title: reportRemoteAssistance 操作
description: 提交报告有效负载的 Post 调用
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 181ac4bdb452fc0746e73cbb0f2679fd152b744e
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60489028"
---
# <a name="reportremoteassistance-action"></a>reportRemoteAssistance 操作

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

提交报告有效负载的 Post 调用

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reportRemoteAssistance
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|属性|类型|说明|
|:---|:---|:---|
|reportingPayload|[remoteAssistanceReporting](../resources/intune-remoteassistance-remoteassistancereporting.md)|尚未记录|



## <a name="response"></a>响应
如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reportRemoteAssistance

Content-type: application/json
Content-length: 1044

{
  "reportingPayload": {
    "@odata.type": "microsoft.graph.remoteAssistanceReporting",
    "id": "Id value",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
    "remoteAssistanceSessionType": "fullControl",
    "helperEmail": "Helper Email value",
    "helperTenantId": "Helper Tenant Id value",
    "helperFirstName": "Helper First Name value",
    "helperLastName": "Helper Last Name value",
    "helperOs": "Helper Os value",
    "helperDeviceAadId": "Helper Device Aad Id value",
    "helperDeviceName": "Helper Device Name value",
    "helperEnrollmentState": "enrolled",
    "sharerEmail": "Sharer Email value",
    "sharerTenantId": "Sharer Tenant Id value",
    "sharerFirstName": "Sharer First Name value",
    "sharerLastName": "Sharer Last Name value",
    "sharerDeviceAadId": "Sharer Device Aad Id value",
    "sharerDeviceName": "Sharer Device Name value",
    "sharerOs": "Sharer Os value",
    "sharerEnrollmentState": "enrolled"
  }
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 204 No Content
```



