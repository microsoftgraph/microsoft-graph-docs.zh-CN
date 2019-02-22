---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb335cd39e6cbcd00f754faae8f7784001c424b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156166"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计算机终结点保护状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|clean|0|计算机干净, 无需任何操作|
|fullScanPending|1|计算机处于挂起的完全扫描状态|
|rebootPending|双面|计算机处于挂起的重新启动状态|
|manualStepsPending|4|计算机处于挂起的手动步骤状态|
|offlineScanPending|utf-8|计算机处于挂起的脱机扫描状态|
|critical|位|计算机处于严重故障状态|




