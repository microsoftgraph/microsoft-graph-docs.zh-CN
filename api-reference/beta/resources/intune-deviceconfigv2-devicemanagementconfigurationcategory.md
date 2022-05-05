---
title: deviceManagementConfigurationCategory 资源类型
description: 设备管理配置策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd8bf0c4f5102f9338673a7b0fdea6f1cc78b5a0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202761"
---
# <a name="devicemanagementconfigurationcategory-resource-type"></a>deviceManagementConfigurationCategory 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备管理配置策略

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementConfigurationCategories](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-list.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 集合|列出 [deviceManagementConfigurationCategory 对象的](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 属性和关系。|
|[获取 deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-get.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|读取 [deviceManagementConfigurationCategory 对象的](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 属性和关系。|
|[创建 deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-create.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|创建新的 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象。|
|[删除 deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-delete.md)|无|删除 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)。|
|[更新 deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-update.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|更新 [deviceManagementConfigurationCategory 对象的](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|项的标识符|
|说明|String|项的说明|
|categoryDescription|String|类别标头的说明|
|helpText|字符串|项的帮助文本|
|name|String|项的名称|
|displayName|String|项的显示名称|
|平台|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|平台类型，类别中的设置有哪些。 可取值为：`none`、`android`、`iOS`、`macOS`、`windows10X`、`windows10`、`linux`、`unknownFutureValue`。|
|技术|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|技术类型，类别中的设置有哪些。 可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`appleRemoteManagement`、`microsoftSense`、`exchangeOnline`、`linuxMdm`、`unknownFutureValue`。|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|指示该类别包含用于符合性或配置的设置。 可取值为：`none`、`configuration`、`compliance`。|
|parentCategoryId|String|类别的父 ID。|
|rootCategoryId|字符串|类别的根 ID。|
|childCategoryIds|String collection|类别的子 ID 列表。|

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
  "categoryDescription": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "platforms": "String",
  "technologies": "String",
  "settingUsage": "String",
  "parentCategoryId": "String",
  "rootCategoryId": "String",
  "childCategoryIds": [
    "String"
  ]
}
```




