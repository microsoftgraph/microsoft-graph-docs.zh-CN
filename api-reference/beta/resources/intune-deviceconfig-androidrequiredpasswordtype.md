---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9112074842e3dc661786acfa6c6c223aa5fe225b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334372"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 必需的密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值, 无意向。|
|字母|1|要求字母密码。|
|字母数字|双面|需要字母数字密码。|
|alphanumericWithSymbols|第三章|需要带符号的字母数字密码。|
|lowSecurityBiometric|4|要求低安全基于生物特征的密码。|
|位数|5|需要数字密码。|
|numericComplex|型|需要数字复杂密码。|
|任意|步|需要密码或模式, 可以接受。|



