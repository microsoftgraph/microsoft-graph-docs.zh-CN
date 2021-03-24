---
title: 更新 deviceComplianceScriptRunSummary
description: 更新 deviceComplianceScriptRunSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7bbd7d35373caaaf9a463955fa3de09025839e38
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130761"
---
# <a name="update-devicecompliancescriptrunsummary"></a>更新 deviceComplianceScriptRunSummary

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceComplianceScriptRunSummary 对象](../resources/intune-devices-devicecompliancescriptrunsummary.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
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
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) 对象的 JSON 表示形式。

下表显示创建 [deviceComplianceScriptRunSummary 时所需的属性](../resources/intune-devices-devicecompliancescriptrunsummary.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|设备合规性脚本运行摘要实体的密钥。 此属性是只读的。|
|noIssueDetectedDeviceCount|Int32|检测脚本未发现问题且设备正常运行的设备数量。 有效值 -2147483648 到 2147483647|
|issueDetectedDeviceCount|Int32|检测脚本发现问题的设备数量。 有效值 -2147483648 到 2147483647|
|detectionScriptErrorDeviceCount|Int32|检测脚本执行遇到错误且未完成的设备数量。 有效值 -2147483648 到 2147483647|
|detectionScriptPendingDeviceCount|Int32|尚未运行最新版本的设备合规性脚本的设备数量。 有效值 -2147483648 到 2147483647|
|lastScriptRunDateTime|DateTimeOffset|脚本跨所有设备的上次运行时间|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "dad42f14-2f14-dad4-142f-d4da142fd4da",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```




