---
title: Microsoft 365浏览器使用情况报告
description: 使用Microsoft 365浏览器使用情况报告深入了解组织中浏览器 (Microsoft Edge、Microsoft Edge 旧版Internet Explorer) 使用情况。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 8b0a0865ecd051d241f41844004ee247e0a57b17
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589770"
---
# <a name="microsoft-365-browser-usage-reports"></a>Microsoft 365浏览器使用情况报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用Microsoft 365浏览器使用情况报告深入了解组织中浏览器 (Microsoft Edge、Microsoft Edge 旧版Internet Explorer) 使用情况。

> **注意：** 有关不同报告视图和名称的详细信息，请参阅Microsoft 365中心 [的报告 - Microsoft 浏览器使用情况](/microsoft-365/admin/activity-reports/browser-usage-report)。

## <a name="reports"></a>报告

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | --------------- | ---------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getbrowseruserdetail.md ) | Stream          | Stream | 获取每个用户的详细浏览器使用情况。  |
| [获取用户数](../api/reportroot-getbrowserusercounts.md ) | Stream          | Stream |获取每个浏览器的活动用户数趋势。 |
| [获取分发用户数](../api/reportroot-getbrowserdistributionusercounts.md) | Stream          | Stream | 按浏览器获取选定时段内的用户数。 |
