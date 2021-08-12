---
title: SharePoint 活动报表
description: SharePoint 活动报表可用于获取每个有权使用 SharePoint 的用户的活动，具体是以用户与文件的交互为依据。 也可以查看以共享文件数为依据的协作级别。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 4c67655dce0bbbe834051a536cb6917111c53fe0729f5430e0558886529edd7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231472"
---
# <a name="sharepoint-activity-reports"></a>SharePoint 活动报表

命名空间：microsoft.graph

SharePoint 活动报表可用于获取每个有权使用 SharePoint 的用户的活动，具体是以用户与文件的交互为依据。 也可以查看以共享文件数为依据的协作级别。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅 Microsoft 365 [reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getsharepointactivityuserdetail.md) | Stream      | 获取用户执行的 SharePoint 活动的详细信息。 |
| [获取文件数](../api/reportroot-getsharepointactivityfilecounts.md) | Stream      | 获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。 |
| [获取用户数](../api/reportroot-getsharepointactivityusercounts.md) | Stream      | 获取活跃用户数趋势。 如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。 |
| [获取页面数](../api/reportroot-getsharepointactivitypages.md) | Stream      | 获取用户访问的唯一页面数。 |

