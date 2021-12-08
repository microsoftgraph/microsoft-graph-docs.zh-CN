---
title: groupPolicySettingMapping 资源类型
description: 到 MDM/Intune 映射的组策略设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4288968bd096a14d8bdbdfea3f25dcaa1409a9e1
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346792"
---
# <a name="grouppolicysettingmapping-resource-type"></a>groupPolicySettingMapping 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

到 MDM/Intune 映射的组策略设置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicySettingMappings](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 集合|列出 [groupPolicySettingMapping 对象的属性和](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 关系。|
|[获取 groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|读取 [groupPolicySettingMapping 对象的属性和](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 关系。|
|[创建 groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|创建新的 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象。|
|[删除 groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|无|删除 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)。|
|[更新 groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|更新 [groupPolicySettingMapping 对象](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|parentId|String|组策略设置的父 ID。|
|childIdList|String collection|组策略设置的子 ID 列表。|
|settingName|String|此组策略设置的名称。|
|settingValue|String|此组策略设置的值。|
|settingValueType|String|此组策略设置的值类型。|
|settingDisplayName|String|此显示名称策略设置的成员。|
|settingDisplayValue|String|此组策略设置的显示值。|
|settingDisplayValueType|String|此组策略设置的显示值类型。|
|settingValueDisplayUnits|String|此组策略设置值的显示单位|
|settingCategory|String|组策略设置位于的类别。|
|mdmCspName|String|此组策略设置映射到的云解决方案提供商名称。|
|mdmSettingUri|String|此组策略设置映射到的 MDM CSP URI。|
|mdmMinimumOSVersion|Int32|此 mdm 设置支持的最低操作系统版本。|
|settingType|[groupPolicySettingType](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|设置类型 (策略的安全性) admx。 可能的值是 `unknown` `policy` `account` ：、、、、、、、、 `securityOptions` `userRightsAssignment` `auditSetting` `windowsFirewallSettings` `appLockerRuleCollection` `dataSourcesSettings` `devicesSettings` `driveMapSettings` `environmentVariables` `filesSettings` `folderOptions` `folders` `iniFiles` `internetOptions` `localUsersAndGroups` `networkOptions` `networkShares` `ntServices` `powerOptions` `printers` `regionalOptionsSettings` `registrySettings` `scheduledTasks` `shortcutSettings` `startMenuSettings` 。|
|isMdmSupported|Boolean|指示 Intune 是否支持该设置|
|mdmSupportedState|[mdmSupportedState](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|指示设置在 Mdm 中是否受支持。 可能的值是：`unknown`、`supported`、`unsupported`、`deprecated`。|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|设置的范围。 可取值为：`unknown`、`device`、`user`。|
|intuneSettingUriList|String collection|此组策略设置映射到的 Intune 设置 URI 列表|
|intuneSettingDefinitionId|String|Intune 设置定义 ID|
|admxSettingDefinitionId|String|Admx 组策略 ID|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicySettingMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "String (identifier)",
  "parentId": "String",
  "childIdList": [
    "String"
  ],
  "settingName": "String",
  "settingValue": "String",
  "settingValueType": "String",
  "settingDisplayName": "String",
  "settingDisplayValue": "String",
  "settingDisplayValueType": "String",
  "settingValueDisplayUnits": "String",
  "settingCategory": "String",
  "mdmCspName": "String",
  "mdmSettingUri": "String",
  "mdmMinimumOSVersion": 1024,
  "settingType": "String",
  "isMdmSupported": true,
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "String"
  ],
  "intuneSettingDefinitionId": "String",
  "admxSettingDefinitionId": "String"
}
```




