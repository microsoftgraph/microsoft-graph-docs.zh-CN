---
title: securityBaselineTemplate 资源类型
description: 帐户的安全基准模板
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8af050df4b90314ad823535860e08557075966df
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319310"
---
# <a name="securitybaselinetemplate-resource-type"></a>securityBaselineTemplate 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

帐户的安全基准模板


继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 securityBaselineTemplates](../api/intune-deviceintent-securitybaselinetemplate-list.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)集合|列出[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性和关系。|
|[获取 securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-get.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|读取[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性和关系。|
|[创建 securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-create.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|创建新的[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象。|
|[删除 securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-delete.md)|无|删除[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)。|
|[更新 securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-update.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|更新[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板 ID|
|displayName|String|从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板的显示名称|
|说明|String|模板的说明继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|versionInfo|String|模板的版本信息继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|isDeprecated|Boolean|模板已弃用或不已弃用。 无法从已弃用的模板创建意向。 继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|intentCount|Int32|从此模板创建的意向数。 继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|模板的类型。 继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。 可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`。|
|publishedDateTime|DateTimeOffset|从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承发布模板时|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|settings|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合|此模板继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)的所有设置的集合|
|categories|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)集合|从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板中的设置类别的集合|
|migratableTo|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)集合|模板集合此模板可从[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)中迁移到继承|
|deviceStateSummary|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|安全基准设备状态摘要|
|deviceStates|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)集合|安全基准设备状态|
|categoryDeviceStateSummaries|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)集合|每个类别的安全基准设备状态摘要|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
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



