---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69d20e06ba23390ff912251bb99980c4a945704c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783709"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计算机终结点保护状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|清理|0|计算机干净，无需任何操作|
|fullScanPending|1|计算机处于挂起的完全扫描状态|
|rebootPending|双面|计算机处于挂起的重新启动状态|
|manualStepsPending|4 |计算机处于挂起的手动步骤状态|
|offlineScanPending|8 |计算机处于挂起的脱机扫描状态|
|关键|16 |计算机处于严重故障状态|



