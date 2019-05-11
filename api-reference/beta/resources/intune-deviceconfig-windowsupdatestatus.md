---
title: windowsUpdateStatus 枚举类型
description: Windows update for business 配置设备状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6eecee6626e4d47856071de3ebb53944e196478
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943639"
---
# <a name="windowsupdatestatus-enum-type"></a>windowsUpdateStatus 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows update for business 配置设备状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|upToDate|0|没有挂起的更新、没有挂起的重新启动更新和没有失败的更新。|
|pendingInstallation|1|存在挂起安装的更新, 其中包括未批准的更新。 没有挂起的重新启动更新, 没有失败的更新。|
|pendingReboot|双面|存在需要重新启动的更新。 没有失败的更新。|
|未能|第三章|无法在设备上安装更新。|




