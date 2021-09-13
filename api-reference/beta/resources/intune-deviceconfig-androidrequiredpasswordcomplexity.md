---
title: androidRequiredPasswordComplexity 枚举类型
description: 可以在 Android 上设置的密码复杂性类型。 其中一个：NONE、LOW、MEDIUM、HIGH。 这是面向 Android 11+的 API。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cdeec66304b60fbf215cca2051a4f8459c691a12
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101707"
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
|low|1|设备上所需的密码复杂性的类型较低，如 Android 文档所定义。|
|中等|2|设备上所需的密码复杂性的类型为中，如 Android 文档所定义。|
|high|3|设备上所需的密码复杂性的类型较高，如 Android 文档所定义。|



