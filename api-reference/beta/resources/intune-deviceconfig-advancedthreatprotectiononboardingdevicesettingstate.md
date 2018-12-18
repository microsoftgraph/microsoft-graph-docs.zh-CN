---
title: advancedThreatProtectionOnboardingDeviceSettingState 资源类型
description: 给定设备 ATP 加入状态。
author: tfitzmac
ms.openlocfilehash: eecdcc1cbaf9c783da6dcf902281aa6394a842a2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310869"
---
# <a name="advancedthreatprotectiononboardingdevicesettingstate-resource-type"></a>advancedThreatProtectionOnboardingDeviceSettingState 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

给定设备 ATP 加入状态。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 advancedThreatProtectionOnboardingDeviceSettingStates](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-list.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)集合|列出属性和[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象之间的关系。|
|[获取 advancedThreatProtectionOnboardingDeviceSettingState](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-get.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|读取属性和[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象的关系。|
|[创建 advancedThreatProtectionOnboardingDeviceSettingState](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-create.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|创建新的[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象。|
|[删除 advancedThreatProtectionOnboardingDeviceSettingState](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-delete.md)|无|删除[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)。|
|[更新 advancedThreatProtectionOnboardingDeviceSettingState](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-update.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|更新[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键|
|platformType|[deviceType](../resources/intune-shared-devicetype.md)|设备平台类型。 可能的值为： `desktop`， `windowsRT`， `winMO6`， `nokia`， `windowsPhone`， `mac`， `winCE`， `winEmbedded`， `iPhone`， `iPad`， `iPod`， `android`， `iSocConsumer`， `unix`， `macMDM`， `holoLens`， `surfaceHub`， `androidForWork`， `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|setting|String|设置类名和属性名。|
|settingName|String|报告的设置名称|
|deviceId|String|报告的设备 ID|
|deviceName|String|报告的设备名称|
|userId|String|报告的用户 ID|
|userEmail|String|报告的用户电子邮件地址|
|userName|String|报告的用户名|
|userPrincipalName|String|报告的用户主体名称|
|deviceModel|String|报告的设备模型|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|设置合规性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|设备合规性宽限期的到期日期/时间|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
  "id": "String (identifier)",
  "platformType": "String",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```





