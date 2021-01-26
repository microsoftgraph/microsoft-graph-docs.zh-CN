---
title: OneDrive 活动报表
description: 通过查看每个许可使用 OneDrive 的用户与 OneDrive 上的文件的交互，你可以获取他们的活动。 它还通过显示共享文件的数量来帮助你了解进行协作的级别。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7d0c069d2787b30f37e634757127b6141843a9ed
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983599"
---
# <a name="onedrive-activity-reports"></a>OneDrive 活动报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过查看每个许可使用 OneDrive 的用户与 OneDrive 上的文件的交互，你可以获取他们的活动。 它还通过显示共享文件的数量来帮助你了解进行协作的级别。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。

## <a name="reports"></a>报告

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getonedriveactivityuserdetail.md) | Stream          | [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) | 获取用户执行的 OneDrive 活动的详细信息。 |
| [获取用户计数](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | 获取 OneDrive 活跃用户数趋势。 |
| [获取文件数](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | 获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。 |


