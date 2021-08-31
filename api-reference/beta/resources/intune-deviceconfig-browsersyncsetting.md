---
title: browserSyncSetting 枚举类型
description: 允许 (未配置) 或 (阻止) 浏览器Microsoft Edge同步。 用于阻止跨设备同步但允许用户替代的选项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ef97db0168971b687d3dac5fb405f5c9482b2a3d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802780"
---
# <a name="browsersyncsetting-enum-type"></a>browserSyncSetting 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

允许 (未配置) 或 (阻止) 浏览器Microsoft Edge同步。 用于阻止跨设备同步但允许用户替代的选项。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值 – 允许跨设备同步浏览器设置。|
|blockedWithUserOverride|1|阻止跨用户设备同步浏览器设置，允许用户替代设置。|
|blocked|2|绝对阻止跨用户设备同步浏览器设置。|



