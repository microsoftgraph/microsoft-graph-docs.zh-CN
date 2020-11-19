---
title: deviceManagementConfigurationCategory 资源类型
description: 设备管理配置策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e2225f24aab8f969a142afdfa1b1aa9ceca9f309
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301545"
---
# <a name="devicemanagementconfigurationcategory-resource-type"></a>deviceManagementConfigurationCategory 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备管理配置策略

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementConfigurationCategories](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-list.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 集合|列出 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象的属性和关系。|
|[获取 deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-get.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|读取 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象的属性和关系。|
|[创建 deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-create.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|创建新的 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象。|
|[删除 deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-delete.md)|无|删除 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)。|
|[更新 deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-update.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|更新 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|项的标识符|
|description|字符串|项目的说明|
|helpText|字符串|项目的帮助文本|
|name|字符串|项目的名称|
|displayName|字符串|项目的显示名称|
|平台|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|平台类型，类别中的设置具有。 可取值为：`none`、`macOS`、`windows10X`、`windows10`。|
|技术|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|技术类型，类别中的设置具有。 可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "String (identifier)",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "platforms": "String",
  "technologies": "String"
}
```




