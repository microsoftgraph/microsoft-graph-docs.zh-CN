---
title: 代码枚举类型
description: 规则验证的错误代码。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 830ab9dac9953791036ea111f7ffe26109c6826e900ff3e2ac660cf171515f71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241924"
---
# <a name="code-enum-type"></a>代码枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

规则验证的错误代码。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无错误。|
|jsonFileInvalid|1 |Json 文件无效错误。|
|jsonFileMissing|2 |Json 文件缺失错误。|
|jsonFileTooLarge|3 |Json 文件太大错误。|
|rulesMissing|4 |规则缺少错误。|
|duplicateRules|5 |重复规则错误。|
|tooManyRulesSpecified|6 |指定错误的规则过多。|
|operatorMissing|7 |运算符缺失错误。|
|operatorNotSupported|8 |运算符不受支持的错误。|
|datatypeMissing|9 |数据类型缺失错误。|
|datatypeNotSupported|10 |数据类型不受支持的错误。|
|operatorDataTypeCombinationNotSupported|11 |运算符数据类型组合不受支持的错误。|
|moreInfoUriMissing|12 |详细信息 urlmissing 错误。|
|moreInfoUriInvalid|13 |详细信息 URL 无效错误。|
|moreInfoUriTooLarge|14 |详细信息 ltoo 大错误。|
|descriptionMissing|15 |说明缺少错误。|
|descriptionInvalid|16 |说明无效错误。|
|descriptionTooLarge|17 |说明太大的错误。|
|titleMissing|18 |标题缺失错误。|
|titleInvalid|19|标题无效错误。|
|titleTooLarge|20|标题太大错误。|
|operandMissing| 21|缺少操作号错误。|
|operandInvalid|22|操作号无效错误。|
|operandTooLarge|23|操作号过大错误。|
|settingNameMissing|24|设置名称缺失错误。|
|settingNameInvalid|25|设置名称无效错误。|
|settingNameTooLarge|26|设置名称过大错误。|
|englishLocaleMissing|27|英语区域设置缺失错误。|
|duplicateLocales|28|区域设置重复错误。|
|unrecognizedLocale|29|无法识别区域设置错误。|
|unknown|30|未知错误。|
|remediationStringsMissing|31|修正字符串缺少错误。|




