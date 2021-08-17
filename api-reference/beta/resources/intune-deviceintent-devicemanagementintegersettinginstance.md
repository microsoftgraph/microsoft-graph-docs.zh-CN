---
title: deviceManagementIntegerSettingInstance 资源类型
description: 表示整数值的设置实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c48e78fbed3d29a6f6852d2fd77b780e8f51f2f49d922433625e9560e0b97f40
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226278"
---
# <a name="devicemanagementintegersettinginstance-resource-type"></a>deviceManagementIntegerSettingInstance 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示整数值的设置实例


继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementIntegerSettingInstances](../api/intune-deviceintent-devicemanagementintegersettinginstance-list.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) 集合|列出 [deviceManagementIntegerSettingInstance 对象的属性和](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) 关系。|
|[获取 deviceManagementIntegerSettingInstance](../api/intune-deviceintent-devicemanagementintegersettinginstance-get.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|读取 [deviceManagementIntegerSettingInstance 对象的属性和](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) 关系。|
|[创建 deviceManagementIntegerSettingInstance](../api/intune-deviceintent-devicemanagementintegersettinginstance-create.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|创建新的 [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) 对象。|
|[删除 deviceManagementIntegerSettingInstance](../api/intune-deviceintent-devicemanagementintegersettinginstance-delete.md)|无|删除 [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)。|
|[更新 deviceManagementIntegerSettingInstance](../api/intune-deviceintent-devicemanagementintegersettinginstance-update.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|更新 [deviceManagementIntegerSettingInstance 对象](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设置实例 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|String|此实例的设置定义的 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|String|值的 JSON 表示形式 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|值|Int32|整数值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntegerSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": 1024
}
```




