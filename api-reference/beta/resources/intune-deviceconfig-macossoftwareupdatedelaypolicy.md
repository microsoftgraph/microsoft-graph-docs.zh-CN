---
title: macOSSoftwareUpdateDelayPolicy 枚举类型
description: 标记 enum 以确定是否延迟 macOS 的软件更新。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 87f4b34447ee8cba65153fcff903239061aef17b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279869"
---
# <a name="macossoftwareupdatedelaypolicy-enum-type"></a>macOSSoftwareUpdateDelayPolicy 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

标记 enum 以确定是否延迟 macOS 的软件更新。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|将不会强制执行软件更新延迟。|
|delayOSUpdateVisibility|1|对 OS 软件更新强制延迟。|
|delayAppUpdateVisibility|双面|对应用软件更新强制延迟。|




