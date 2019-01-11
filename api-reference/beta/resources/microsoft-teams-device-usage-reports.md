---
title: Microsoft Teams 设备使用情况报告
description: '使用 Microsoft 团队设备使用率报告您的组织中获取的 Microsoft 团队设备用法见解。 '
localization_priority: Normal
ms.openlocfilehash: e89b5b133b8ebb64a59dfffe75ba9b47d2bf0c7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826157"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams 设备使用情况报告

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。 在 Microsoft Graph 中国由 21Vianet 不支持这些 Api。

使用 Microsoft 团队设备使用率报告您的组织中获取的 Microsoft 团队设备用法见解。 

## <a name="methods"></a>方法

| 方法                                   | 返回类型                              | 说明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。 |
| [获取用户计数](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | 按设备类型获取每日唯一用户数。 |
| [获取分发用户计数](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | 在选定的时间段内按设备类型获取唯一用户数。 |
