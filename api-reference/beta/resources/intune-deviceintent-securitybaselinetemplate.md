---
title: securityBaselineTemplate 资源类型
description: 帐户的安全基线模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 906f351dc79e0f624e2baf26138ad559418005f2
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58263812"
---
# <a name="securitybaselinetemplate-resource-type"></a>securityBaselineTemplate 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

帐户的安全基线模板


继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 securityBaselineTemplates](../api/intune-deviceintent-securitybaselinetemplate-list.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) 集合|列出 [securityBaselineTemplate 对象的属性和](../resources/intune-deviceintent-securitybaselinetemplate.md) 关系。|
|[获取 securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-get.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|读取 [securityBaselineTemplate 对象的属性和](../resources/intune-deviceintent-securitybaselinetemplate.md) 关系。|
|[创建 securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-create.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|创建新的 [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) 对象。|
|[删除 securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-delete.md)|无|删除 [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)。|
|[更新 securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-update.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|更新 [securityBaselineTemplate 对象](../resources/intune-deviceintent-securitybaselinetemplate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|模板 ID 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|displayName|String|模板的模板显示名称继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|description|String|模板的说明 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|versionInfo|字符串|模板的版本信息 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|isDeprecated|布尔值|模板是否被弃用。 无法从已弃用模板创建意图。 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|intentCount|Int32|从此模板创建的意图数。 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|模板的类型。 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。 可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`、`deviceCompliance`、`deviceConfigurationForOffice365`、`cloudPC`、`firewallSharedSettings`。|
|platformType|[policyPlatformType](../resources/intune-deviceintent-policyplatformtype.md)|模板的平台。 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。|
|templateSubtype|[deviceManagementTemplateSubtype](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|模板的子类型。 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。 可取值为：`none`、`firewall`、`diskEncryption`、`attackSurfaceReduction`、`endpointDetectionReponse`、`accountProtection`、`antivirus`、`firewallSharedAppList`、`firewallSharedIpList`、`firewallSharedPortlist`。|
|publishedDateTime|DateTimeOffset|发布模板时 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|设置|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) 集合|此模板继承自 [deviceManagementTemplate 的所有设置的集合](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|categories|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) 集合|模板中的设置类别集合 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|migratableTo|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) 集合|此模板可以迁移到的模板集合 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|deviceStateSummary|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|安全基线设备状态摘要|
|deviceStates|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 集合|安全基线设备状态|
|categoryDeviceStateSummaries|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 集合|每个类别设备状态摘要的安全基线|

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
  "platformType": "String",
  "templateSubtype": "String",
  "publishedDateTime": "String (timestamp)"
}
```




