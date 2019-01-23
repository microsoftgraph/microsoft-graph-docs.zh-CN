---
title: windowsUpdateType 枚举类型
description: 分支的设备将接收从其更新
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d3dd0f6d8ba46d7f1cc803b217a98a862602149
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400135"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

分支的设备将接收从其更新

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|允许用户设置。|
|all|1|半年 （目标） 通道。 设备从半年通道 （目标） 中获取所有适用的功能更新。|
|businessReadyOnly|2|半年通道。 设备获取更新功能从半年通道。|
|windowsInsiderBuildFast|3|Windows 内幕生成-Fast|
|windowsInsiderBuildSlow|4|Windows 内幕生成-速度较慢|
|windowsInsiderBuildRelease|5|Windows 内幕发布版本|




