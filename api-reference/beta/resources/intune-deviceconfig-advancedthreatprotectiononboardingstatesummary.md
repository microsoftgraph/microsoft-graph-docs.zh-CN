---
title: advancedThreatProtectionOnboardingStateSummary 资源类型
description: Windows帐户的 defender 高级威胁防护载入状态摘要。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1ca587b9ac7a0c886f54260c53329334fa72e27
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101791"
---
# <a name="advancedthreatprotectiononboardingstatesummary-resource-type"></a>advancedThreatProtectionOnboardingStateSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows帐户的 defender 高级威胁防护载入状态摘要。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 advancedThreatProtectionOnboardingStateSummary](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|读取 [advancedThreatProtectionOnboardingStateSummary 对象的属性和](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) 关系。|
|[更新 advancedThreatProtectionOnboardingStateSummary](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-update.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|更新 [advancedThreatProtectionOnboardingStateSummary 对象](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|唯一标识符|
|unknownDeviceCount|Int32|未知设备的数量|
|notApplicableDeviceCount|Int32|不适用设备的数量|
|compliantDeviceCount|Int32|兼容设备的数量|
|remediatedDeviceCount|Int32|已修复设备的数量|
|nonCompliantDeviceCount|Int32|不兼容设备的数量|
|errorDeviceCount|Int32|错误设备的数量|
|conflictDeviceCount|Int32|冲突设备的数量|
|notAssignedDeviceCount|Int32|未分配设备的数量|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|advancedThreatProtectionOnboardingDeviceSettingStates|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) 集合|尚未记录|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notAssignedDeviceCount": 1024
}
```



