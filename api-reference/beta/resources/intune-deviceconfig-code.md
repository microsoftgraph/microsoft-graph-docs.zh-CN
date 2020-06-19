---
title: 代码枚举类型
description: 规则验证的错误代码。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 86a1e90ae6b52ca6b6a4fa6cc02403d426329ce5
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789376"
---
# <a name="code-enum-type"></a>代码枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

规则验证的错误代码。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无错误。|
|jsonFileInvalid|1 |Json 文件无效错误。|
|jsonFileMissing|双面|Json 文件缺少错误。|
|jsonFileTooLarge|第三章|Json 文件过大错误。|
|rulesMissing|4 |缺少错误的规则。|
|duplicateRules|5 |重复规则错误。|
|tooManyRulesSpecified|6 |指定的规则过多错误。|
|operatorMissing|7 |运算符缺少错误。|
|operatorNotSupported|8 |运算符不受支持错误。|
|datatypeMissing|9 |数据类型缺少错误。|
|datatypeNotSupported|10  |数据类型不受支持错误。|
|operatorDataTypeCombinationNotSupported|11x17|运算符数据类型组合不受支持错误。|
|moreInfoUriMissing|12 |详细信息 urlmissing 错误。|
|moreInfoUriInvalid|13 |详细信息 url 无效错误。|
|moreInfoUriTooLarge|14 |详细信息您的 ltoo 大错误。|
|descriptionMissing|15 |Description 缺少错误。|
|descriptionInvalid|16 |Description 无效错误。|
|descriptionTooLarge|17 |Description 过大错误。|
|titleMissing|18 |缺少标题错误。|
|titleInvalid|合|标题无效错误。|
|titleTooLarge|20|"标题太大" 错误。|
|operandMissing| 21|操作数缺少错误。|
|operandInvalid|22|操作数无效错误。|
|operandTooLarge|上午|操作数过大错误。|
|settingNameMissing|24|设置名称缺少错误。|
|settingNameInvalid|word|设置名称无效错误。|
|settingNameTooLarge|26|设置名称太大错误。|
|englishLocaleMissing|27|英语区域设置缺少错误。|
|duplicateLocales|28|重复区域设置错误。|
|unrecognizedLocale|29|无法识别的区域设置错误。|
|unknown|30|未知错误。|
|remediationStringsMissing|31|修正字符串缺少错误。|



