---
title: deviceComplianceSettingState 资源类型
description: 给定设备的设备符合性设置状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d618356d115f437bccccee57f6c259a1cdbd14a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403033"
---
# <a name="devicecompliancesettingstate-resource-type"></a>deviceComplianceSettingState 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的设备符合性设置状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComplianceSettingStates](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 集合|列出 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。|
|[获取 deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|读取 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。|
|[创建 deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。|
|[删除 deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|无|删除 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)。|
|[更新 deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。|

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
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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




