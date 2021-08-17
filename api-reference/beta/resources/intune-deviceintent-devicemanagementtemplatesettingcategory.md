---
title: deviceManagementTemplateSettingCategory 资源类型
description: 表示模板设置类别的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db744fc2b5888881cef52962fbe259354a47f62142afa8ed7d8bd2ae0a5a349c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139444"
---
# <a name="devicemanagementtemplatesettingcategory-resource-type"></a>deviceManagementTemplateSettingCategory 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示模板设置类别的实体


继承自 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementTemplateSettingCategories](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-list.md)|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) 集合|列出 [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) 对象的属性和关系。|
|[获取 deviceManagementTemplateSettingCategory](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-get.md)|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|读取 [deviceManagementTemplateSettingCategory 对象的属性和](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) 关系。|
|[创建 deviceManagementTemplateSettingCategory](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-create.md)|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|创建新的 [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) 对象。|
|[删除 deviceManagementTemplateSettingCategory](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-delete.md)|无|删除 [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)。|
|[更新 deviceManagementTemplateSettingCategory](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-update.md)|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|更新 [deviceManagementTemplateSettingCategory 对象](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|类别 ID 继承自 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|displayName|字符串|类别名称 继承自 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|hasRequiredSetting|布尔值|类别包含顶级所需设置 继承自 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 集合|此类别的设置定义包含继承自 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|recommendedSettings|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) 集合|此类别包含的设置|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplateSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "hasRequiredSetting": true
}
```




