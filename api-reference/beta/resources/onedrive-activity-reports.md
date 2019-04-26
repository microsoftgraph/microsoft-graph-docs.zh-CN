---
title: OneDrive 活动报表
description: 您可以通过查看其与 onedrive 上的文件的交互, 获取获得使用 onedrive 的每个用户的活动。 它还可帮助您了解通过显示共享文件数而进行的协作级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3a99ba5dbc1a61b11d916c9fff90cec53a4eeaf9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345521"
---
# <a name="onedrive-activity-reports"></a>OneDrive 活动报表

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以通过查看其与 onedrive 上的文件的交互, 获取获得使用 onedrive 的每个用户的活动。 它还可帮助您了解通过显示共享文件数而进行的协作级别。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getonedriveactivityuserdetail.md) | Stream          | [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) | 获取用户执行的 OneDrive 活动的详细信息。 |
| [获取用户数](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | 获取 OneDrive 活跃用户数趋势。 |
| [获取文件数](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | 获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。 |
