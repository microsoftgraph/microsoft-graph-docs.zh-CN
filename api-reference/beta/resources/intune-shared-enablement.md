---
title: 启用枚举类型
description: '用于指示状态的设备的值。 '
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c77da7026640e9ad0a6f6f08f077d509cb411f22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888254"
---
# <a name="enablement-enum-type"></a>启用枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于指示状态的设备的值。 

请注意，没有区别禁用，且未配置。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|设备默认值，没有用途。|
|enabled|1|允许在设备上的设置。|
|禁用|2|禁用在设备上的设置。|
