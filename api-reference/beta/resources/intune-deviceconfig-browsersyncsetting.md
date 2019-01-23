---
title: browserSyncSetting 枚举类型
description: Allow(Not Configured) 或 prevent(Block) Microsoft 边缘浏览器设置同步。 选项可以防止同步跨设备，但允许用户替代。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dce2b82b1eea5e4b06ed0f6949ba6a403b073a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431320"
---
# <a name="browsersyncsetting-enum-type"></a>browserSyncSetting 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Allow(Not Configured) 或 prevent(Block) Microsoft 边缘浏览器设置同步。 选项可以防止同步跨设备，但允许用户替代。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值 – 允许跨设备同步的浏览器设置。|
|blockedWithUserOverride|1|防止跨用户设备同步的浏览器设置时，允许用户替代的设置。|
|已阻止|2|绝对防止跨用户设备同步的浏览器设置。|




