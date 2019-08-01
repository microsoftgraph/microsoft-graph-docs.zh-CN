---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d7630e3cac3702380da07c2a92857d9f2786810a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027571"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 枚举类型

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



