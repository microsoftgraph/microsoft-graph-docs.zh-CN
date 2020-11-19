---
title: deviceManagementScriptUserState 资源类型
description: 包含设备管理脚本的用户运行状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0fdf91765d6387a735439ad4bcf66f568f3944ab
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267598"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>deviceManagementScriptUserState 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备管理脚本的用户运行状态的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementScriptUserStates](../api/intune-devices-devicemanagementscriptuserstate-list.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 集合|列出 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象的属性和关系。|
|[获取 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|读取 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象的属性和关系。|
|[创建 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|创建新的 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象。|
|[删除 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|无|删除 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)。|
|[更新 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|更新 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|设备管理脚本用户状态实体的键。 此属性是只读的。|
|successDeviceCount|Int32|特定用户的成功设备计数。|
|errorDeviceCount|Int32|特定用户的错误设备计数。|
|userPrincipalName|字符串|特定用户的用户主体名称。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 集合|此脚本在特定用户的所有设备上的运行状态列表。|

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




