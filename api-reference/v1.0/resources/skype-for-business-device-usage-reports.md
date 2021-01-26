---
title: Skype for Business 设备使用情况报表
description: Skype for Business 设备使用情况报表可用于获取整个组织中使用的客户端和设备类型的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: f0e46f94141691a17c5f7636f497c3f03fef71df
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980638"
---
# <a name="skype-for-business-device-usage-reports"></a>Skype for Business 设备使用情况报表

命名空间：microsoft.graph

Skype for Business 设备使用情况报表可用于获取整个组织中使用的客户端和设备类型的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。

> **注意：** 有关不同报告视图和名称的详细信息，请参阅 [Microsoft 365 报告 - 使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。

## <a name="reports"></a>报告

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | Stream      | 获取用户的 Skype for Business 设备使用情况的详细信息。 |
| [获取分发用户数](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | Stream      | 获取组织中使用唯一设备的用户数。 报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。 |
| [获取用户计数](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | Stream      | 获取使用情况趋势，即组织中有多少用户已使用 Skype for Business 应用进行了连接。 还可以按设备类型（Windows、Windows 手机、Android 手机、iPhone 或 iPad）进一步了解整个组织中安装和使用的 Skype for Business 客户端应用。 |

