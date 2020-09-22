---
title: OneDrive 使用情况报表
description: 您可以从在组织的所有 OneDrive 帐户中使用的文件总数和存储量中获取您从 OneDrive 获取的值的高级视图。 然后，可以向下钻取活跃 OneDrive 帐户的趋势、用户已交互的文件数以及使用的存储空间。 它还提供了每个 OneDrive 帐户的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 57f91b1821624f933e87c7de49053ef873179f7d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979369"
---
# <a name="onedrive-usage-reports"></a>OneDrive 使用情况报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以从在组织的所有 OneDrive 帐户中使用的文件总数和存储量中获取您从 OneDrive 获取的值的高级视图。 然后，可以向下钻取活跃 OneDrive 帐户的趋势、用户已交互的文件数以及使用的存储空间。 它还提供了每个 OneDrive 帐户的详细信息。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表-OneDrive For business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | ---------------------------------------- | ---------------------------------------- |
| [获取帐户详细信息](../api/reportroot-getonedriveusageaccountdetail.md) | Stream          | [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) | 获取帐户的 OneDrive 使用情况的详细信息。 |
| [获取帐户数](../api/reportroot-getonedriveusageaccountcounts.md) | Stream          | [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) | 获取 OneDrive for Business 活跃网站数趋势。 用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。 |
| [获取文件数](../api/reportroot-getonedriveusagefilecounts.md) | Stream          | [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) | 获取跨所有网站的文件总数和活跃文件数。 如果文件在指定时间段内被保存、同步、修改或共享，则视为活跃文件。 |
| [获取存储](../api/reportroot-getonedriveusagestorage.md) | Stream          | [siteUsageStorage](../resources/siteusagestorage.md) | 获取 OneDrive for Business 使用的存储空间趋势。 |


