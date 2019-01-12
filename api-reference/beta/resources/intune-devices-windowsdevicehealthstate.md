---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 628450b33a219e8408d5c5887c6902b78ae02bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923941"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

计算机终结点保护状态
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|clean|0|计算机的完全而不不需要任何操作|
|fullScanPending|1|计算机处于挂起完全扫描状态|
|rebootPending|2|计算机处于挂起的重新启动状态|
|manualStepsPending|4|计算机处于挂起的手动步骤状态|
|offlineScanPending|8|计算机处于挂起脱机扫描状态|
|critical|16|计算机处于关键失败状态|





