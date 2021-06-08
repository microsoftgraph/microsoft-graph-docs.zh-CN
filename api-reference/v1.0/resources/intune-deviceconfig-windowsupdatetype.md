---
title: windowsUpdateType 枚举类型
description: 哪些分支设备将接收其更新
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f49158686884d55825751a9314a50a9ab9a16d57
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759943"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

哪些分支设备将接收其更新

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|all|1|半年频道 (定向) 。 设备从半年频道和目标用户获取 (功能) 。|
|businessReadyOnly|2|半年频道。 设备从半年频道获取功能更新。|
|windowsInsiderBuildFast|3|Windows预览体验成员内部版本 - 快速|
|windowsInsiderBuildSlow|4 |Windows预览体验成员内部版本 - 慢|
|windowsInsiderBuildRelease|5 |预览Windows内部版本|




