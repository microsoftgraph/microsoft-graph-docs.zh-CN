---
title: securityBaselineSettingState 资源类型
description: 设备设置的安全基准合规性状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab5dd14c0929c58b9c076d1115d487e560d80333
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522578"
---
# <a name="securitybaselinesettingstate-resource-type"></a>securityBaselineSettingState 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备设置的安全基准合规性状态

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 securityBaselineSettingStates](../api/intune-deviceintent-securitybaselinesettingstate-list.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)集合|列出[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象的属性和关系。|
|[获取 securityBaselineSettingState](../api/intune-deviceintent-securitybaselinesettingstate-get.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)|读取[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象的属性和关系。|
|[创建 securityBaselineSettingState](../api/intune-deviceintent-securitybaselinesettingstate-create.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)|创建新的[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象。|
|[删除 securityBaselineSettingState](../api/intune-deviceintent-securitybaselinesettingstate-delete.md)|无|删除[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)。|
|[更新 securityBaselineSettingState](../api/intune-deviceintent-securitybaselinesettingstate-update.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)|更新[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的唯一标识符|
|settingName|String|报告的设置名称|
|state|[securityBaselineComplianceState](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|安全基准设置的符合性状态。 可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。|
|settingCategoryId|String|此设置所属的设置类别 id|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "String (identifier)",
  "settingName": "String",
  "state": "String",
  "settingCategoryId": "String"
}
```



