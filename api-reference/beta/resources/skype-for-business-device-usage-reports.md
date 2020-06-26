---
title: Skype for Business 设备使用情况报表
description: 您可以获取有关在组织中使用的客户端和设备的类型的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 09472ef74e1f28a683a8fef340f451f75b539175
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896782"
---
# <a name="skype-for-business-device-usage-reports"></a>Skype for Business 设备使用情况报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以获取有关在组织中使用的客户端和设备的类型的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-使用的 Skype For business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | Stream          | [skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md) | 获取用户的 Skype for Business 设备使用情况的详细信息。 |
| [获取分发用户数](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | Stream          | [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) | 获取组织中使用唯一设备的用户数。 报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。 |
| [获取用户数](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | Stream          | [skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md) | 获取使用情况趋势，即组织中有多少用户已使用 Skype for Business 应用进行了连接。 还可以按设备类型（Windows、Windows 手机、Android 手机、iPhone 或 iPad）进一步了解整个组织中安装和使用的 Skype for Business 客户端应用。 |
