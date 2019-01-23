---
title: deviceManagementScriptUserState 资源类型
description: 包含运行状态的设备管理脚本的用户的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1884967707be8e126724148afa5d04b07f80a48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407282"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>deviceManagementScriptUserState 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含运行状态的设备管理脚本的用户的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 deviceManagementScriptUserStates](../api/intune-devices-devicemanagementscriptuserstate-list.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合|列出属性和[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象之间的关系。|
|[获取 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|读取属性和[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的关系。|
|[创建 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|创建新的[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。|
|[删除 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|无|删除[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)。|
|[更新 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|更新[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备管理脚本的用户状态实体的键。|
|successDeviceCount|Int32|成功的特定用户的设备计数。|
|errorDeviceCount|Int32|错误的特定用户的设备计数。|
|userPrincipalName|String|特定用户的用户主体名称。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合|此脚本的特定用户的所有设备上的运行状态的列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "userPrincipalName": "String"
}
```




