---
title: OneDrive 使用情况报表
description: OneDrive 使用情况报表可用于大致了解 OneDrive 带来的价值，具体是以跨组织中所有 OneDrive 帐户的文件总数和存储为依据。 然后，可以向下钻取活跃 OneDrive 帐户的趋势、用户已交互的文件数以及使用的存储空间。 这些报表还提供每个 OneDrive 帐户的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 22ed2e491bb8ed2631968d35490ca902fce93e4b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980988"
---
# <a name="onedrive-usage-reports"></a>OneDrive 使用情况报表

命名空间：microsoft.graph

OneDrive 使用情况报表可用于大致了解 OneDrive 带来的价值，具体是以跨组织中所有 OneDrive 帐户的文件总数和存储为依据。 然后，可以向下钻取活跃 OneDrive 帐户的趋势、用户已交互的文件数以及使用的存储空间。 这些报表还提供每个 OneDrive 帐户的详细信息。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。

## <a name="reports"></a>报告

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | ---------------------------------------- |
| [获取帐户详细信息](../api/reportroot-getonedriveusageaccountdetail.md) | Stream      | 获取帐户的 OneDrive 使用情况的详细信息。 |
| [获取帐户数](../api/reportroot-getonedriveusageaccountcounts.md) | Stream      | 获取 OneDrive for Business 活跃网站数趋势。 用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。 |
| [获取文件数](../api/reportroot-getonedriveusagefilecounts.md) | Stream      | 获取跨所有网站的文件总数和活跃文件数。 如果文件在指定时间段内被保存、同步、修改或共享，则视为活跃文件。 |
| [获取存储](../api/reportroot-getonedriveusagestorage.md) | Stream      | 获取 OneDrive for Business 使用的存储空间趋势。 |

