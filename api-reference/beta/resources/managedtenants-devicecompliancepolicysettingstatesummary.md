---
title: deviceCompliancePolicySettingStateSummary 资源类型
description: 表示给定托管租户的设备合规性策略设置状态摘要。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 02b69b5df1c6ae482c653960a0081bc078be815d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402067"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>deviceCompliancePolicySettingStateSummary 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示给定托管租户的设备合规性策略设置状态摘要。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceCompliancePolicySettingStateSummary](../api/managedtenants-managedtenant-list-devicecompliancepolicysettingstatesummary.md)|[microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 集合|获取 [deviceCompliancePolicySettingStateSummary 对象](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 及其属性的列表。|
|[获取 deviceCompliancePolicySettingStateSummary](../api/managedtenants-devicecompliancepolicysettingstatesummary-get.md)|[microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|读取 [deviceCompliancePolicySettingStateSummary 对象的属性和](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符。 必填。 只读。|
|conflictDeviceCount|Int32|冲突状态中的设备数。 可选。 只读。|
|errorDeviceCount|Int32|出现错误状态的设备数。 可选。 只读。|
|failedDeviceCount|Int32|故障状态中的设备数。 可选。 只读。|
|intuneAccountId|String|帐户标识Microsoft Intune标识。 必填。 只读。|
|intuneSettingId|String|Intune 设置的标识符。 可选。 只读。|
|lastRefreshedDateTime|DateTimeOffset|实体上次在多租户管理平台中更新的日期和时间。 可选。 只读。|
|notApplicableDeviceCount|Int32|状态不适用的设备数量。 可选。 只读。|
|pendingDeviceCount|Int32|挂起状态的设备数。 可选。 只读。|
|policyType|String|设备合规性策略的类型。 可选。 只读。|
|settingName|String|设备合规性策略中设置的名称。 可选。 只读。|
|succeededDeviceCount|Int32|状态成功的设备数。 可选。 只读。|
|tenantDisplayName|String|托管显示名称租户的租户。 必填。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 必填。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "conflictDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "intuneAccountId": "String",
  "intuneSettingId": "String",
  "notApplicableDeviceCount": "Integer",
  "pendingDeviceCount": "Integer",
  "policyType": "String",
  "settingName": "String",
  "succeededDeviceCount": "Integer",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
