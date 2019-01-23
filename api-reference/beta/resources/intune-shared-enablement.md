---
title: 启用枚举类型
description: 介绍 Intune，支持多个工作流 Microsoft Graph API 启用枚举。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 538b52790cf7748453adfda2a6bea8334a36fb87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399561"
---
# <a name="enablement-enum-type"></a>启用枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于指示状态的设备的值。 

请注意，没有区别禁用，且未配置。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，没有用途。|
|enabled|1|允许在设备上的设置。|
|禁用|2|禁用在设备上的设置。|
