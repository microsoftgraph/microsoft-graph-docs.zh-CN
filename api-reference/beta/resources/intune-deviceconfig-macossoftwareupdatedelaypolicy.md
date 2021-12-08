---
title: macOSSoftwareUpdateDelayPolicy 枚举类型
description: 用于确定是否延迟 macOS 软件更新的标志枚举。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dc7fa44a86f4b10ca3f49172b86ee3bfdb336da8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339890"
---
# <a name="macossoftwareupdatedelaypolicy-enum-type"></a>macOSSoftwareUpdateDelayPolicy 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于确定是否延迟 macOS 软件更新的标志枚举。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|不会强制执行软件更新延迟。|
|delayOSUpdateVisibility|1|强制延迟操作系统软件更新。|
|delayAppUpdateVisibility|2|强制延迟应用软件更新。|
|unknownFutureValue|4|Sentinel 成员，适用于客户端无法处理新枚举值的情况。|
|delayMajorOsUpdateVisibility|8 |强制延迟主要操作系统软件更新。|




