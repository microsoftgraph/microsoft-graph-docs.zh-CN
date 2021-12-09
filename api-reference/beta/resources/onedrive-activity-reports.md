---
title: OneDrive 活动报表
description: 通过查看每个授权使用 OneDrive 用户与文件上的交互，OneDrive。 它还通过显示共享的文件数来帮助您了解进行协作的级别。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 188cb9ff8fc6750a1beb4177a82e3c1135da20bb
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390792"
---
# <a name="onedrive-activity-reports"></a>OneDrive 活动报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过查看每个授权使用 OneDrive 用户与文件上的交互，OneDrive。 它还通过显示共享的文件数来帮助您了解进行协作的级别。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅 Microsoft 365 [reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。

## <a name="reports"></a>报告

| 函数                                                     | CSV 返回类型 | JSON 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [获取用户详细信息](../api/reportroot-getonedriveactivityuserdetail.md) | Stream          | Stream           | 获取用户执行的 OneDrive 活动的详细信息。                 |
| [获取用户数](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | Stream           | 获取 OneDrive 活跃用户数趋势。        |
| [获取文件数](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | Stream           | 获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。 |


