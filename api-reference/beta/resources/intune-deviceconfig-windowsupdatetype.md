---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35b117b1a64650a475d392ffadf81769d3b0b08b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978666"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

将从哪些分支设备接收其更新

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|允许用户进行设置。|
|各种|1|半年频道 (定向)。 设备从半年频道 (定向) 获取所有适用的功能更新。|
|businessReadyOnly|双面|半年频道。 设备从半年频道获取功能更新。|
|windowsInsiderBuildFast|第三章|Windows 预览体验成员内部版本-快速|
|windowsInsiderBuildSlow|4|Windows 预览体验成员内部版本-慢|
|windowsInsiderBuildRelease|5|发布 Windows 预览体验成员内部版本|





