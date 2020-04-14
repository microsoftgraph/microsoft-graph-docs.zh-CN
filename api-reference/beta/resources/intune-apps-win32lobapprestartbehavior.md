---
title: win32LobAppRestartBehavior 枚举类型
description: 指示重新启动操作的类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2902f3808ea1ebcc1442b0675c89da51b059f2c2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422637"
---
# <a name="win32lobapprestartbehavior-enum-type"></a>win32LobAppRestartBehavior 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示重新启动操作的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|basedOnReturnCode|0|如果操作返回重新启动代码，则在运行应用程序安装后，Intune 将重新启动设备。|
|允许|1|Intune 不会对由应用安装引起的重新启动代码执行任何特定操作。 Intune 不会尝试取消对 MSI 应用的重新启动。|
|强制|双面|Intune 将尝试取消对 MSI 应用的重新启动。|
|有效|第三章|Intune 将强制在应用程序安装操作完成后立即重新启动设备。|



