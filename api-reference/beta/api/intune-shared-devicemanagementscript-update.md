---
title: 更新 deviceManagementScript
description: 更新 deviceManagementScript 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c36f2eeb63908edb503829f92b782f4b31ea20c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791312"
---
# <a name="update-devicemanagementscript"></a>更新 deviceManagementScript

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的属性。

## <a name="prerequisites"></a>先决条件
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）||
| &nbsp;&nbsp;**设备管理** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp;**策略集** | DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序||
| &nbsp;&nbsp;**设备管理** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp;**策略集** | DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的 JSON 表示形式。

下表显示创建[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|设备管理脚本的唯一标识符。|
|displayName|字符串|设备管理脚本的名称。|
|说明|String|设备管理脚本的可选说明。|
|runSchedule|runSchedule|脚本运行的间隔。 如果未定义，脚本将运行一次|
|scriptContent|Binary|脚本内容。|
|createdDateTime|DateTimeOffset|设备管理脚本的创建日期和时间。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|上次修改设备管理脚本的日期和时间。 此属性是只读的。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文的类型。 可取值为：`system`、`user`。|
|enforceSignatureCheck|布尔值|指示是否需要检查脚本签名。|
|fileName|String|脚本文件名。|
|roleScopeTagIds|String collection|此 PowerShellScript 实例的范围标记 Id 的列表。|
|runAs32Bit|布尔值|一个指示 PowerShell 脚本是否应作为32位运行的值|



## <a name="response"></a>响应
如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
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
  "runAs32Bit": true
}
```

### <a name="response"></a>响应
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
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
  "runAs32Bit": true
}
```






