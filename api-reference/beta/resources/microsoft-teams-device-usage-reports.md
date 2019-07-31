---
title: Microsoft Teams 设备使用情况报告
description: '使用 Microsoft 团队设备使用情况报告可深入了解组织中的 Microsoft 团队设备使用情况。 '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0beada44b46afad1b8a51358f18259374a654f14
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966711"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams 设备使用情况报告

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 Microsoft 团队设备使用情况报告可深入了解组织中的 Microsoft 团队设备使用情况。 

## <a name="methods"></a>方法

| 方法                                   | 返回类型                              | 说明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。 |
| [获取用户计数](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | 按设备类型获取每日唯一用户数。 |
| [获取分发用户计数](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | 在选定的时间段内按设备类型获取唯一用户数。 |
