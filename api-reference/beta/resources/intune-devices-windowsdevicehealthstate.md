---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3a12ac4e09981e21b51d97109f72569cafe628ba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999603"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计算机终结点保护状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|清理|0|计算机干净, 无需任何操作|
|fullScanPending|1|计算机处于挂起的完全扫描状态|
|rebootPending|双面|计算机处于挂起的重新启动状态|
|manualStepsPending|4|计算机处于挂起的手动步骤状态|
|offlineScanPending|utf-8|计算机处于挂起的脱机扫描状态|
|关键|位|计算机处于严重故障状态|





