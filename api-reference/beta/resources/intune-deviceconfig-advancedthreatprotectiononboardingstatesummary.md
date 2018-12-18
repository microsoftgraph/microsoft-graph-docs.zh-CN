---
title: advancedThreatProtectionOnboardingStateSummary 资源类型
description: Windows defender 高级的威胁保护入职培训状态摘要跨帐户。
author: tfitzmac
ms.openlocfilehash: 3a31d489374b87469d2ed6fb87bb70f8d89d710c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359169"
---
# <a name="advancedthreatprotectiononboardingstatesummary-resource-type"></a>advancedThreatProtectionOnboardingStateSummary 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows defender 高级的威胁保护入职培训状态摘要跨帐户。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 advancedThreatProtectionOnboardingStateSummary](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|读取属性和[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的关系。|
|[更新 advancedThreatProtectionOnboardingStateSummary](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-update.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|更新[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的属性。|

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
|notAssignedDeviceCount|Int32|未分配的设备数|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|advancedThreatProtectionOnboardingDeviceSettingStates|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)集合|尚未记录|

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





