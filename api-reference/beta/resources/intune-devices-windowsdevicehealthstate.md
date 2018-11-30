---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
ms.openlocfilehash: 601531dd71ee0d44e9f5ebc89eb018ba5e0f2675
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041340"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

计算机终结点保护状态
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|clean|0|计算机的完全而不不需要任何操作|
|fullScanPending|1|计算机处于挂起完全扫描状态|
|rebootPending|2|计算机处于挂起的重新启动状态|
|manualStepsPending|4|计算机处于挂起的手动步骤状态|
|offlineScanPending|8|计算机处于挂起脱机扫描状态|
|critical|16|计算机处于关键失败状态|





