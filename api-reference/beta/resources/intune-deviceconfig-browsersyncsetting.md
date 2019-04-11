---
title: browserSyncSetting 枚举类型
description: 允许 (未配置) 或阻止 (阻止) Microsoft Edge 浏览器设置的同步。 选项可阻止跨设备同步, 但允许用户重写。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f08031e970f56c071a4dd01af0542bd56924edd5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789743"
---
# <a name="browsersyncsetting-enum-type"></a>browserSyncSetting 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

允许 (未配置) 或阻止 (阻止) Microsoft Edge 浏览器设置的同步。 选项可阻止跨设备同步, 但允许用户重写。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值–允许跨设备同步浏览器设置。|
|blockedWithUserOverride|1|阻止跨用户设备同步浏览器设置, 允许用户重写设置。|
|堵塞|双面|绝对阻止跨用户设备同步浏览器设置。|





