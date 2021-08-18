---
title: deviceComplianceScriptRuleError 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30b828904ed3cdd63fa1495e010126bb5b20e4e76b7cdc22cb9221f80d81ce77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54161309"
---
# <a name="devicecompliancescriptruleerror-resource-type"></a>deviceComplianceScriptRuleError 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录


继承自 [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|code|[code](../resources/intune-deviceconfig-code.md)|错误代码。 继承自 [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)。 可能的值是 `none` `jsonFileInvalid` ：、、、、、、、 `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` 。|
|deviceComplianceScriptRulesValidationError|[deviceComplianceScriptRulesValidationError](../resources/intune-deviceconfig-devicecompliancescriptrulesvalidationerror.md)|错误代码。 继承自 [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)。 可能的值是 `none` `jsonFileInvalid` ：、、、、、、、 `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` 。|
|message|String|错误消息。 继承自 [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)|
|settingName|String|设置出错规则的名称。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRuleError",
  "code": "String",
  "deviceComplianceScriptRulesValidationError": "String",
  "message": "String",
  "settingName": "String"
}
```




