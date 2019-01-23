---
title: windowsUpdateStatus 枚举类型
description: Windows 更新的业务配置设备状态
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74493359eeccdbc6df1c351ecec771b5990649b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431384"
---
# <a name="windowsupdatestatus-enum-type"></a>windowsUpdateStatus 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 更新的业务配置设备状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|upToDate|0|待处理更新，没有挂起的重新启动更新和没有失败的更新。|
|pendingInstallation|1|有的待处理的安装，其中包括未批准的更新的更新。 有任何挂起的重新启动更新、 没有失败的更新。|
|pendingReboot|2|有需要重新启动的更新。 不存在失败的更新。|
|failed|3|有未能在设备上安装更新。|




