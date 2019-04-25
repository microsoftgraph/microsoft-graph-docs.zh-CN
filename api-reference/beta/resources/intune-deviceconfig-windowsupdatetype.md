---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 228cc5ba4b50681bfe78a15ef214d6f3ab2ebb17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523593"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

将从哪些分支设备接收其更新

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|允许用户进行设置。|
|各种|1|半年频道 (定向)。 设备从半年频道 (定向) 获取所有适用的功能更新。|
|businessReadyOnly|2 |半年频道。 设备从半年频道获取功能更新。|
|windowsInsiderBuildFast|3 |Windows 预览体验成员内部版本-快速|
|windowsInsiderBuildSlow|4 |Windows 预览体验成员内部版本-慢|
|windowsInsiderBuildRelease|5 |发布 Windows 预览体验成员内部版本|





