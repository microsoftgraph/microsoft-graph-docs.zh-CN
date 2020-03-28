---
title: 更新 deviceShellScript
description: 更新 deviceShellScript 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9e3c2da2008b5e44f4b13449abd6b63251fe08f
ms.sourcegitcommit: d93fcc2212491567f8322b1cc0c02d37829b6051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/28/2020
ms.locfileid: "43034746"
---
# <a name="update-deviceshellscript"></a>更新 deviceShellScript

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性。

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
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的 JSON 表示形式。

下表显示创建[deviceShellScript](../resources/intune-devices-deviceshellscript.md)时所需的属性。

|属性|类型|Description|
|:---|:---|:---|
|executionFrequency|持续时间|脚本运行的间隔。 如果未定义，则脚本将运行一次。|
|retryCount|Int32|脚本失败时重试脚本的次数。|
|blockExecutionNotifications|Boolean|指示在脚本运行时是否通知用户。|
|id|字符串|设备管理脚本的唯一标识符。|
|displayName|字符串|设备管理脚本的名称。|
|description|String|设备管理脚本的可选说明。|
|scriptContent|Binary|脚本内容。|
|createdDateTime|DateTimeOffset|设备管理脚本的创建日期和时间。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|上次修改设备管理脚本的日期和时间。 此属性是只读的。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文的类型。 可取值为：`system`、`user`。|
|fileName|String|脚本文件名。|
|roleScopeTagIds|String 集合|此 PowerShellScript 实例的范围标记 Id 的列表。|



## <a name="response"></a>响应
如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "PT2M43.444327S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "PT2M43.444327S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "id": "ca9e0ad8-0ad8-ca9e-d80a-9ecad80a9eca",
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```



