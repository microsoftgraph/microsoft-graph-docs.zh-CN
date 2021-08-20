---
title: deviceManagementBooleanSettingInstance 资源类型
description: 表示布尔值的设置实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b91f4798290802e3f0ed1d019a47c309324bf1b2d4071dd8ef5a6e90416f3e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54219890"
---
# <a name="devicemanagementbooleansettinginstance-resource-type"></a>deviceManagementBooleanSettingInstance 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示布尔值的设置实例


继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementBooleanSettingInstances](../api/intune-deviceintent-devicemanagementbooleansettinginstance-list.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) 集合|列出 [deviceManagementBooleanSettingInstance 对象的属性和](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) 关系。|
|[获取 deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-get.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|读取 [deviceManagementBooleanSettingInstance 对象的属性和](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) 关系。|
|[创建 deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-create.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|创建新的 [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) 对象。|
|[删除 deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-delete.md)|无|删除 [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)。|
|[更新 deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-update.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|更新 [deviceManagementBooleanSettingInstance 对象](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设置实例 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|String|此实例的设置定义的 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|String|值的 JSON 表示形式 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|Boolean|布尔值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementBooleanSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": true
}
```




