---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件所需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c1f4ece497d4d8370a7e444e0c47c7181d6c1da3c05f24398f3520a795e9585b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54153179"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a>androidWorkProfileRequiredPasswordType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 工作配置文件所需的密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意图。|
|lowSecurityBiometric|1 |需要低安全生物识别密码。|
|必需|2 |必需。|
|atLeastNumeric|3 |至少需要数字密码。|
|numericComplex|4 |需要数字复杂密码。|
|atLeastAlphabetic|5 |至少需要字母密码。|
|atLeastAlphanumeric|6 |至少需要字母数字密码。|
|alphanumericWithSymbols|7 |至少包含需要符号密码的字母数字。|




