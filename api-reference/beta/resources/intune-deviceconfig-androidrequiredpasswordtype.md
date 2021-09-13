---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2e4931cef836f446613c54b3c9eb3eaf9506de24
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101679"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 所需的密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意图。|
|字母|1|需要字母密码。|
|alphanumeric|2|需要字母数字密码。|
|alphanumericWithSymbols|3|需要符号密码的字母数字。|
|lowSecurityBiometric|4 |需要低安全生物识别密码。|
|numeric|5 |需要数字密码。|
|numericComplex|6 |需要数字复杂密码。|
|任意|7 |密码或模式是必需的，任何密码或模式都是可接受的。|



