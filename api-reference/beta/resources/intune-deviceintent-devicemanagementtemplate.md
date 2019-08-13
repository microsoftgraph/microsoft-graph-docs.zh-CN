---
title: deviceManagementTemplate 资源类型
description: 表示已定义的设备设置集合的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3e2c7536c61bfaf8287a0a2428e0b861e09f3a5f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337620"
---
# <a name="devicemanagementtemplate-resource-type"></a>deviceManagementTemplate 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示已定义的设备设置集合的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementTemplates](../api/intune-deviceintent-devicemanagementtemplate-list.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)集合|列出[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性和关系。|
|[获取 deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|读取[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性和关系。|
|[创建 deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|创建新的[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。|
|[删除 deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|无|删除[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。|
|[更新 deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|更新[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性。|
|[createInstance 操作](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|尚未记录|
|[compare 函数](../api/intune-deviceintent-devicemanagementtemplate-compare.md)|[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|模板 ID|
|displayName|String|模板的显示名称|
|说明|String|模板的说明|
|versionInfo|String|模板的版本信息|
|isDeprecated|Boolean|模板已弃用或不已弃用。 无法从已弃用的模板创建意向。|
|intentCount|Int32|从此模板创建的意向数。|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|模板的类型。 可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`。|
|publishedDateTime|DateTimeOffset|发布模板时|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|settings|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合|此模板包含的所有设置的集合|
|categories|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)集合|模板中设置类别的集合|
|migratableTo|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)集合|此模板可以迁移到的模板集合|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "versionInfo": "String",
  "isDeprecated": true,
  "intentCount": 1024,
  "templateType": "String",
  "publishedDateTime": "String (timestamp)"
}
```



