---
title: deviceManagementScriptUserState 资源类型
description: 包含运行状态的设备管理脚本的用户的属性。
author: tfitzmac
ms.openlocfilehash: acce3d40d390c22d848b9ee3f8c94c997ae6da12
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301209"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>deviceManagementScriptUserState 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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
|id|字符串|设备管理脚本的用户状态实体的键。|
|successDeviceCount|Int32|成功的特定用户的设备计数。|
|errorDeviceCount|Int32|错误的特定用户的设备计数。|
|userPrincipalName|字符串|特定用户的用户主体名称。|

## <a name="relationships"></a>Relationships
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





