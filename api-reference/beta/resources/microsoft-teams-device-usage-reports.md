---
title: Microsoft Teams 设备使用情况报告
description: '使用 Microsoft Teams 设备使用情况报告深入了解组织中 Microsoft Teams 设备使用情况。 '
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7be5d8d0d369d9cff0fe295f8765a5e4f3ca28bc
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980786"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams 设备使用情况报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 Microsoft Teams 设备使用情况报告深入了解组织中 Microsoft Teams 设备使用情况。 

## <a name="methods"></a>方法

| 方法                                   | 返回类型                              | 说明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。 |
| [获取用户计数](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | 按设备类型获取每日唯一用户数。 |
| [获取分发用户计数](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | 在选定的时间段内按设备类型获取唯一用户数。 |


