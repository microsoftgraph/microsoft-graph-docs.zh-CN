---
title: windowsUpdateStatus 枚举类型
description: Windows update for business 配置设备状态
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ac307aae8f43cd423c41c1a20ccbc7b9928452d3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441091"
---
# <a name="windowsupdatestatus-enum-type"></a>windowsUpdateStatus 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows update for business 配置设备状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|upToDate|0|没有挂起的更新、没有挂起的重新启动更新和没有失败的更新。|
|pendingInstallation|1|存在挂起安装的更新，其中包括未批准的更新。 没有挂起的重新启动更新，没有失败的更新。|
|pendingReboot|双面|存在需要重新启动的更新。 没有失败的更新。|
|未能|第三章|无法在设备上安装更新。|



