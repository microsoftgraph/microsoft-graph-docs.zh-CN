---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ebe11f91b90074839a1a03dab2ce79788f259358
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208056"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




