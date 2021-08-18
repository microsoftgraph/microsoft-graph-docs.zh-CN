---
title: deviceManagementSettingCategory 资源类型
description: 表示设置类别的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da2f35c8a068fd794e187c559b829772088731602d2b2d55f42bd76754098428
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54156217"
---
# <a name="devicemanagementsettingcategory-resource-type"></a>deviceManagementSettingCategory 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示设置类别的实体

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementSettingCategories](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) 集合|列出 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) 对象的属性和关系。|
|[获取 deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|读取 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) 对象的属性和关系。|
|[创建 deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|创建新的 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) 对象。|
|[删除 deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|无|删除 [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)。|
|[更新 deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|更新 [deviceManagementSettingCategory 对象](../resources/intune-deviceintent-devicemanagementsettingcategory.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|类别 ID|
|displayName|字符串|类别名称|
|hasRequiredSetting|布尔值|类别包含所需的顶级设置|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 集合|此类别包含的设置定义|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "hasRequiredSetting": true
}
```




