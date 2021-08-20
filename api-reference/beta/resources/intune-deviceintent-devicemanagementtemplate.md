---
title: deviceManagementTemplate 资源类型
description: 表示定义的设备设置集合的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b119ddbfb175b8cd80cd2174e0ffbf5f724e1fe
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262632"
---
# <a name="devicemanagementtemplate-resource-type"></a>deviceManagementTemplate 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示定义的设备设置集合的实体

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementTemplates](../api/intune-deviceintent-devicemanagementtemplate-list.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) 集合|列出 [deviceManagementTemplate 对象的属性和](../resources/intune-deviceintent-devicemanagementtemplate.md) 关系。|
|[获取 deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|读取 [deviceManagementTemplate 对象的属性和](../resources/intune-deviceintent-devicemanagementtemplate.md) 关系。|
|[创建 deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|创建新的 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) 对象。|
|[删除 deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|无|删除 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。|
|[更新 deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|更新 [deviceManagementTemplate 对象](../resources/intune-deviceintent-devicemanagementtemplate.md) 的属性。|
|[createInstance 操作](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|尚未记录|
|[compare 函数](../api/intune-deviceintent-devicemanagementtemplate-compare.md)|[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) 集合|尚未记录|
|[importOffice365DeviceConfigurationPolicies 操作](../api/intune-deviceintent-devicemanagementtemplate-importoffice365deviceconfigurationpolicies.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|模板 ID|
|displayName|String|模板的显示名称|
|description|String|模板的说明|
|versionInfo|String|模板的版本信息|
|isDeprecated|布尔值|模板是否被弃用。 无法从已弃用模板创建意图。|
|intentCount|Int32|从此模板创建的意图数。|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|模板的类型。 可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`、`deviceCompliance`、`deviceConfigurationForOffice365`、`cloudPC`、`firewallSharedSettings`。|
|platformType|[policyPlatformType](../resources/intune-deviceintent-policyplatformtype.md)|模板的平台。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。|
|templateSubtype|[deviceManagementTemplateSubtype](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|模板的子类型。 可取值为：`none`、`firewall`、`diskEncryption`、`attackSurfaceReduction`、`endpointDetectionReponse`、`accountProtection`、`antivirus`、`firewallSharedAppList`、`firewallSharedIpList`、`firewallSharedPortlist`。|
|publishedDateTime|DateTimeOffset|模板发布时间|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|设置|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) 集合|此模板具有的所有设置的集合|
|categories|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) 集合|模板中的设置类别集合|
|migratableTo|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) 集合|此模板可以迁移到的模板集合|

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
  "platformType": "String",
  "templateSubtype": "String",
  "publishedDateTime": "String (timestamp)"
}
```




