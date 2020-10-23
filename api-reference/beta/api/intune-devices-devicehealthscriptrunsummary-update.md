---
title: 更新 deviceHealthScriptRunSummary
description: 更新 deviceHealthScriptRunSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2b1d00b523e989d927e834b54f8b748bb93d301
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729206"
---
# <a name="update-devicehealthscriptrunsummary"></a>更新 deviceHealthScriptRunSummary

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) 对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) 对象的 JSON 表示形式。

下表显示创建 [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|设备运行状况脚本的键运行摘要实体。 此属性是只读的。|
|noIssueDetectedDeviceCount|Int32|检测脚本找不到问题且设备正常运行的设备数|
|issueDetectedDeviceCount|Int32|检测脚本发现问题的设备数|
|detectionScriptErrorDeviceCount|Int32|检测脚本执行时遇到错误且未完成的设备数量|
|detectionScriptPendingDeviceCount|Int32|尚未运行的设备运行状况脚本的最新版本的设备数量|
|issueRemediatedDeviceCount|Int32|修正脚本能够解决检测到的问题的设备数|
|remediationSkippedDeviceCount|Int32|跳过修正的设备数|
|issueReoccurredDeviceCount|Int32|已成功执行修正脚本但未能解决检测到的问题的设备数量|
|remediationScriptErrorDeviceCount|Int32|修正脚本执行时遇到错误且未完成的设备数量|
|lastScriptRunDateTime|DateTimeOffset|在所有设备上的脚本的上次运行时间|
|issueRemediatedCumulativeDeviceCount|Int32|最近30天内修正的设备数量|



## <a name="response"></a>响应
如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-type: application/json
Content-length: 494

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "8221b043-b043-8221-43b0-218243b02182",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```





