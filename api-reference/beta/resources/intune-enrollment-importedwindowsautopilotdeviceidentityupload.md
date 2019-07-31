---
title: importedWindowsAutopilotDeviceIdentityUpload 资源类型
description: 使用上载导入 windows autopilot 设备。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e9f0ac008f945edf94a0ca9d2b21a34b551c52c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999078"
---
# <a name="importedwindowsautopilotdeviceidentityupload-resource-type"></a>importedWindowsAutopilotDeviceIdentityUpload 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

使用上载导入 windows autopilot 设备。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|列出 importedWindowsAutopilotDeviceIdentityUploads|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)集合|列出[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的属性和关系。|
|获取 importedWindowsAutopilotDeviceIdentityUpload|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|读取[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的属性和关系。|
|创建 importedWindowsAutopilotDeviceIdentityUpload|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|创建新的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象。|
|删除 importedWindowsAutopilotDeviceIdentityUpload|无|删除[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)。|
|更新 importedWindowsAutopilotDeviceIdentityUpload|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|更新[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的属性。|
|Importedwindowsautopilotdeviceidentityupload 函数|String|创建具有 autopilot 设备流的上载请求。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|createdDateTimeUtc|DateTimeOffset|创建实体时的日期/时间。|
|status|[importedWindowsAutopilotDeviceIdentityUploadStatus](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|上载状态。 可取值为：`noUpload`、`pending`、`complete`、`error`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 集合|作为此上载的一部分的所有 Autopilot 设备的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "String (identifier)",
  "createdDateTimeUtc": "String (timestamp)",
  "status": "String"
}
```





