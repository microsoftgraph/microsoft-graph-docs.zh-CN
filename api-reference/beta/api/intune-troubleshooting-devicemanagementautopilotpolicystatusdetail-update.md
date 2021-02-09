---
title: 更新 deviceManagementAutopilotPolicyStatusDetail
description: 更新 deviceManagementAutopilotPolicyStatusDetail 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8e38d9ae11c0eb34d92681725fcd3173e2d9a9b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155627"
---
# <a name="update-devicemanagementautopilotpolicystatusdetail"></a>更新 deviceManagementAutopilotPolicyStatusDetail

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceManagementAutopilotPolicyStatusDetail 对象](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceManagementAutopilotPolicyStatusDetail 对象的](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) JSON 表示形式。

下表显示创建 [deviceManagementAutopilotPolicyStatusDetail 时所需的属性](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID|
|displayName|String|策略的友好名称。|
|policyType|[deviceManagementAutopilotPolicyType](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|策略的类型。 可取值为：`unknown`、`application`、`appModel`、`configurationPolicy`。|
|complianceStatus|[deviceManagementAutopilotPolicyComplianceStatus](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|策略合规性状态。 可取值为：`unknown`、`compliant`、`installed`、`notCompliant`、`notInstalled`、`error`。|
|trackedOnEnrollmentStatus|布尔|指示此许可是否作为 autopilot bootstrap 注册同步会话的一部分进行跟踪|
|lastReportedDateTime|DateTimeOffset|报告的策略状态的时间戳|
|errorCode|Int32|与策略的合规性或强制状态相关联的错误模式。 强制状态的错误代码优先（如果存在）。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "errorCode": 9
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "dbe093ee-93ee-dbe0-ee93-e0dbee93e0db",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "errorCode": 9
}
```




