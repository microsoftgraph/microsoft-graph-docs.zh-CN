---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cd4556abb04e3895b31ca52fa87eab4d3dfdd90b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58816555"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 所需的密码类型。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意图。|
|字母|1|需要字母密码。|
|alphanumeric|2|需要字母数字密码。|
|alphanumericWithSymbols|3|需要符号密码的字母数字。|
|lowSecurityBiometric|4 |需要低安全生物识别密码。|
|numeric|5 |需要数字密码。|
|numericComplex|6 |需要数字复杂密码。|
|任意|7 |密码或模式是必需的，任何密码或模式都是可接受的。|



