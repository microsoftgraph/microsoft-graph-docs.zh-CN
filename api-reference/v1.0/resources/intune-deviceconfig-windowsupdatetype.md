---
title: windowsUpdateType 枚举类型
description: 哪些分支设备将从中接收其更新
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7f1417e59137dd67d0b9c757141e064d909b4c20
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734219"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

哪些分支设备将从中接收其更新

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|全部|1|半年频道 (目标) 。 设备从半年频道 (目标) 获取所有适用的功能更新。|
|businessReadyOnly|2|半年频道。 设备从半年频道获取功能更新。|
|windowsInsiderBuildFast|3|Windows 预览体验成员版本 - 快速|
|windowsInsiderBuildSlow|4|Windows 预览体验成员版本 - 慢|
|windowsInsiderBuildRelease|5|发布 Windows 预览体验成员版本|





