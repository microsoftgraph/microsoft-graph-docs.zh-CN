---
title: groupPolicySettingMapping 资源类型
description: MDM/Intune 映射的组策略设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db235993f9ddb87c11407136676608ab8d1c1992
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298650"
---
# <a name="grouppolicysettingmapping-resource-type"></a>groupPolicySettingMapping 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MDM/Intune 映射的组策略设置。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 groupPolicySettingMappings](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 集合|列出 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象的属性和关系。|
|[获取 groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|读取 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象的属性和关系。|
|[创建 groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|创建新的 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象。|
|[删除 groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|无|删除 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)。|
|[更新 groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|更新 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|尚未记录|
|parentId|字符串|组策略设置的父 Id。|
|childIdList|String 集合|组策略设置的子 Id 列表。|
|settingName|String|此组策略设置的名称。|
|settingValue|字符串|此组策略设置的值。|
|settingValueType|字符串|此组策略设置的值类型。|
|settingDisplayName|字符串|此组策略设置的显示名称。|
|settingDisplayValue|字符串|此组策略设置的显示值。|
|settingDisplayValueType|字符串|此组策略设置的显示值类型。|
|settingValueDisplayUnits|字符串|此组策略设置值的显示单位|
|settingCategory|字符串|组策略设置所属的类别。|
|mdmCspName|字符串|将此组策略设置映射到的 CSP 名称。|
|mdmSettingUri|字符串|将此组策略设置映射到的 MDM CSP URI。|
|mdmMinimumOSVersion|Int32|此 mdm 设置支持的最低 OS 版本。|
|settingType|[groupPolicySettingType](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|组策略的设置类型 (安全性或 admx) 。 可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。|
|isMdmSupported|Boolean|指示此设置是否由 Intune 支持|
|mdmSupportedState|[mdmSupportedState](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|指示是否支持 Mdm 中的设置。 可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|设置的范围。 可取值为：`unknown`、`device`、`user`。|
|intuneSettingUriList|String 集合|此组策略设置映射到的 Intune 设置 Uri 列表|
|intuneSettingDefinitionId|字符串|Intune 设置定义 Id|
|admxSettingDefinitionId|字符串|Admx 组策略 Id|

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




