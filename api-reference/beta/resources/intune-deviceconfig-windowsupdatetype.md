---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 71a1c43cdcb0668f903871cc1bd1a680beee80e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039606"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

将从哪些分支设备接收其更新

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|允许用户进行设置。|
|各种|1 |目标) 的半年频道 (。 设备将从半年频道 (目标) 获取所有适用的功能更新。|
|businessReadyOnly|2 |半年频道。 设备从半年频道获取功能更新。|
|windowsInsiderBuildFast|第三章|Windows 预览体验成员内部版本-快速|
|windowsInsiderBuildSlow|4 |Windows 预览体验成员内部版本-慢|
|windowsInsiderBuildRelease|5 |发布 Windows 预览体验成员内部版本|






