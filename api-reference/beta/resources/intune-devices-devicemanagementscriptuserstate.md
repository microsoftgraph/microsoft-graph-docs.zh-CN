---
title: deviceManagementScriptUserState 资源类型
description: 包含设备管理脚本的用户运行状态的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 683084b1505c91718e10661e8605c6c8fa7003b7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125960"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>deviceManagementScriptUserState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备管理脚本的用户运行状态的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementScriptUserStates](../api/intune-devices-devicemanagementscriptuserstate-list.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 集合|列出 [deviceManagementScriptUserState 对象的属性和](../resources/intune-devices-devicemanagementscriptuserstate.md) 关系。|
|[获取 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|读取 [deviceManagementScriptUserState 对象的属性和](../resources/intune-devices-devicemanagementscriptuserstate.md) 关系。|
|[创建 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|创建新的 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象。|
|[删除 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|无|删除 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)。|
|[更新 deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|更新 [deviceManagementScriptUserState 对象](../resources/intune-devices-devicemanagementscriptuserstate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备管理脚本用户状态实体的键。 此属性是只读的。|
|successDeviceCount|Int32|特定用户的成功设备计数。|
|errorDeviceCount|Int32|特定用户的错误设备计数。|
|userPrincipalName|String|特定用户的用户原则名称。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 集合|此脚本跨特定用户的所有设备的运行状态列表。|

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



