---
title: win32LobAppRestartBehavior 枚举类型
description: 指示重新启动操作的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d850410b5380864988b9bd43abed41d9729138dbecd7d11f615da063a2b21c7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54153256"
---
# <a name="win32lobapprestartbehavior-enum-type"></a>win32LobAppRestartBehavior 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示重新启动操作的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|basedOnReturnCode|0|如果操作返回重启代码，Intune 将在运行应用安装后重新启动设备。|
|allow|1 |Intune 不会对应用安装生成的重启代码执行任何特定操作。 Intune 不会尝试禁止为 MSI 应用重启。|
|suppress|2 |Intune 将尝试禁止为 MSI 应用重启。|
|force|3 |Intune 将强制设备在应用安装操作后立即重新启动。|




