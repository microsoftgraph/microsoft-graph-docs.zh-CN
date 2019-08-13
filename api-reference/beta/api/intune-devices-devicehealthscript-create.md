---
title: 创建 deviceHealthScript
description: 创建新的 deviceHealthScript 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0084852f4c0cb236931ee532f12e54a08c1e2fc2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311639"
---
# <a name="create-devicehealthscript"></a>创建 deviceHealthScript

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象。

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
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中, 提供 deviceHealthScript 对象的 JSON 表示形式。

下表显示创建 deviceHealthScript 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|设备管理脚本的唯一标识符。 继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|displayName|字符串|设备管理脚本的名称。 继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|说明|String|设备管理脚本的可选说明。 继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|脚本运行的间隔。 如果未定义, 脚本将在从[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)继承后运行。|
|scriptContent|Binary|脚本内容。 继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|createdDateTime|DateTimeOffset|设备管理脚本的创建日期和时间。 继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改设备管理脚本的日期和时间。 继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文的类型。 继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)。 可取值为：`system`、`user`。|
|enforceSignatureCheck|Boolean|指示是否需要检查脚本签名。 继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|fileName|String|脚本文件名。 继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|roleScopeTagIds|String collection|此 PowerShellScript 实例的范围标记 Id 的列表。 继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|runAs32Bit|Boolean|一个指示 PowerShell 脚本是否应作为从[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)继承的32位运行的值|
|complianceRule|[deviceHealthScriptComplianceRule](../resources/intune-devices-devicehealthscriptcompliancerule.md)|尚未记录|
|remediationScriptContent|Binary|尚未记录|
|runRemediationScript|Boolean|尚未记录|



## <a name="response"></a>响应
如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```






