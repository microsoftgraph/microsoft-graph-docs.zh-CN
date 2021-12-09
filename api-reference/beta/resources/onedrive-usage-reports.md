---
title: OneDrive 使用情况报表
description: 你可以获取从 OneDrive 获取的值的高级别视图，以表示组织中所有 OneDrive 帐户使用的文件总数和存储。 然后，可以向下钻取活跃 OneDrive 帐户的趋势、用户已交互的文件数以及使用的存储空间。 它还为你提供每个帐户OneDrive详细信息。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 6219126a872af35d2c6a2f757e80ebe440ed8898
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390681"
---
# <a name="onedrive-usage-reports"></a>OneDrive 使用情况报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以获取从 OneDrive 获取的值的高级别视图，以表示组织中所有 OneDrive 帐户使用的文件总数和存储。 然后，可以向下钻取活跃 OneDrive 帐户的趋势、用户已交互的文件数以及使用的存储空间。 它还为你提供每个帐户OneDrive详细信息。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报表 -](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)OneDrive for Business使用情况。

## <a name="reports"></a>报告

| 函数                                                     | CSV 返回类型 | JSON 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :-------------- | ---------------- | ------------------------------------------------------------ |
| [获取帐户详细信息](../api/reportroot-getonedriveusageaccountdetail.md) | Stream          | Stream           | 获取帐户的 OneDrive 使用情况的详细信息。                 |
| [获取帐户数](../api/reportroot-getonedriveusageaccountcounts.md) | Stream          | Stream           | 获取 OneDrive for Business 活跃网站数趋势。 用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。 |
| [获取文件数](../api/reportroot-getonedriveusagefilecounts.md) | Stream          | Stream           | 获取跨所有网站的文件总数和活跃文件数。 如果文件在指定时间段内被保存、同步、修改或共享，则视为活跃文件。 |
| [获取存储](../api/reportroot-getonedriveusagestorage.md)  | Stream          | Stream           | 获取 OneDrive for Business 使用的存储空间趋势。 |


