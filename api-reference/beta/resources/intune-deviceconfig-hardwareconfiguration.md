---
title: hardwareConfiguration 资源类型
description: Intune 将为客户提供在已注册的 windows 10 和已加入Azure Active Directory配置硬件/bios 设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d19f8f3b8efc3d60fb60bce18851a072a50d8895
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345422"
---
# <a name="hardwareconfiguration-resource-type"></a>hardwareConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Intune 将为客户提供在已注册的 windows 10 和已加入Azure Active Directory配置硬件/bios 设置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 hardwareConfigurations](../api/intune-deviceconfig-hardwareconfiguration-list.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) 集合|列出 [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) 对象的属性和关系。|
|[获取 hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-get.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|读取 [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) 对象的属性和关系。|
|[创建 hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-create.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|创建新的 [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) 对象。|
|[删除 hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-delete.md)|None|删除 [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)。|
|[更新 hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-update.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|更新 [hardwareConfiguration 对象](../resources/intune-deviceconfig-hardwareconfiguration.md) 的属性。|
|[分配操作](../api/intune-deviceconfig-hardwareconfiguration-assign.md)|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|硬件配置的唯一标识符|
|version|Int32|硬件配置的版本|
|displayName|String|硬件配置的名称|
|description|String|硬件配置说明|
|createdDateTime|DateTimeOffset|创建硬件配置的时间戳。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|修改硬件配置的时间戳。 此属性是只读的。|
|fileName|String|硬件配置的文件名|
|configurationFileContent|Binary|硬件配置的文件内容|
|hardwareConfigurationFormat|[hardwareConfigurationFormat](../resources/intune-deviceconfig-hardwareconfigurationformat.md)|硬件配置的 Oem 类型。 可取值为：`dell`、`surface`、`surfaceDock`。|
|roleScopeTagIds|字符串集合|硬件配置的范围标记标识列表|
|perDevicePasswordDisabled|布尔|一个值，指示是否禁用每个开发密码|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md) 集合|硬件配置的组分配列表|
|runSummary|[hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|硬件配置的运行摘要|
|deviceRunStates|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) 集合|跨所有设备的硬件配置的运行状态列表|
|userRunStates|[hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md) 集合|所有用户的硬件配置的运行状态列表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfiguration",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "fileName": "String",
  "configurationFileContent": "binary",
  "hardwareConfigurationFormat": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "perDevicePasswordDisabled": true
}
```




