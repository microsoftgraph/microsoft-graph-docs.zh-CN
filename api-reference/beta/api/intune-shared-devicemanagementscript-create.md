---
title: 创建 deviceManagementScript
description: 创建新的 deviceManagementScript 对象。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d077f34cef3c75680c48229680c76f0a045694c9
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867810"
---
# <a name="create-devicemanagementscript"></a>创建 deviceManagementScript

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）||
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp;**策略集** | DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序||
| &nbsp; &nbsp; **设备管理** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp;**策略集** | DeviceManagementManagedDevices.ReadWrite.All|

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
在请求正文中，提供 deviceManagementScript 对象的 JSON 表示形式。

下表显示创建 deviceManagementScript 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|设备管理脚本的唯一标识符。|
|displayName|String|设备管理脚本的名称。|
|说明|String|设备管理脚本的可选说明。|
|scriptContent|二进制|脚本内容。|
|createdDateTime|DateTimeOffset|创建设备管理脚本的日期和时间。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|上次修改设备管理脚本的日期和时间。 此属性是只读的。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文的类型。 可取值为：`system`、`user`。|
|enforceSignatureCheck|Boolean|指示是否需要检查脚本签名。|
|fileName|String|脚本文件名。|
|roleScopeTagIds|String 集合|此 PowerShellScript 实例的范围标记标识列表。|
|runAs32Bit|Boolean|指示 PowerShell 脚本是否应该作为 32 位运行的值|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
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
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
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







