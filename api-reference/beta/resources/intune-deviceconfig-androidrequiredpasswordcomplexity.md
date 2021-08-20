---
title: androidRequiredPasswordComplexity 枚举类型
description: 可以在 Android 上设置的密码复杂性类型。 其中一个：NONE、LOW、MEDIUM、HIGH。 这是面向 Android 11+的 API。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e852542516ee07c5f32bf166dddce25e68e672923bff8698869c135410495754
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239929"
---
# <a name="androidrequiredpasswordcomplexity-enum-type"></a>androidRequiredPasswordComplexity 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

可以在 Android 上设置的密码复杂性类型。 其中一个：NONE、LOW、MEDIUM、HIGH。 这是面向 Android 11+的 API。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|设备默认值，无密码。|
|low|1 |设备上所需的密码复杂性的类型较低，如 Android 文档所定义。|
|中等|2 |设备上所需的密码复杂性的类型为中，如 Android 文档所定义。|
|high|3 |设备上所需的密码复杂性的类型较高，如 Android 文档所定义。|




