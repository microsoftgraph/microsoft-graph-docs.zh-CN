---
title: importedWindowsAutopilotDeviceIdentity 资源类型
description: 导入 Windows AutoPilot 的设备。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9fef97ac8e39a6f816c685673cc27ec1f9d59a71
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986130"
---
# <a name="importedwindowsautopilotdeviceidentity-resource-type"></a>importedWindowsAutopilotDeviceIdentity 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

导入 Windows AutoPilot 的设备。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 importedWindowsAutopilotDeviceIdentities](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-list.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 集合|列表属性和[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象关系。|
|[获取 importedWindowsAutopilotDeviceIdentity](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-get.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|阅读属性和关系[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象。|
|[Create importedWindowsAutopilotDeviceIdentity](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-create.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|创建新[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)对象。|
|[删除 importedWindowsAutopilotDeviceIdentity](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-delete.md)|无|删除[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)。|
|[更新 importedWindowsAutopilotDeviceIdentity](../api/intune-enrollment-importedwindowsautopilotdeviceidentity-update.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|更新 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|对象的 GUID|
|orderIdentifier|字符串|Windows autopilot 设备订单 Id。|
|serialNumber|字符串|Windows autopilot 设备序列号。|
|productKey|字符串|Windows autopilot 设备产品密钥。|
|hardwareIdentifier|Binary|Windows autopilot 设备硬件 Blob。|
|state|[importedWindowsAutopilotDeviceIdentityState](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|导入设备的当前状态。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "orderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "hardwareIdentifier": "binary",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "String",
    "deviceRegistrationId": "String",
    "deviceErrorCode": 1024,
    "deviceErrorName": "String"
  }
}
```



