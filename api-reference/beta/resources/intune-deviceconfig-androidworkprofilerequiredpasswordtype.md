---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件所需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8de2a525a2fbca9fa8398a0d991643a28a9ae2ea
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58816730"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a>androidWorkProfileRequiredPasswordType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 工作配置文件所需的密码类型。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意图。|
|lowSecurityBiometric|1|需要低安全生物识别密码。|
|必需|2|必填。|
|atLeastNumeric|3|至少需要数字密码。|
|numericComplex|4 |需要数字复杂密码。|
|atLeastAlphabetic|5 |至少需要字母密码。|
|atLeastAlphanumeric|6 |至少需要字母数字密码。|
|alphanumericWithSymbols|7 |至少包含需要符号密码的字母数字。|



