---
title: Yammer 活动报表
description: 你可以了解组织与 Yammer 的交互级别，包括整个组织生成的活动数以及发布、喜欢和阅读 Yammer 上邮件的唯一用户数。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 5d157217c94d35450929745a4f5bf0989bb2bf49
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390827"
---
# <a name="yammer-activity-reports"></a>Yammer 活动报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以了解组织与 Yammer 的交互级别，包括整个组织生成的活动数以及发布、喜欢和阅读 Yammer 上邮件的唯一用户数。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅 Microsoft 365 [reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。

## <a name="reports"></a>报告

| 函数                                                     | CSV 返回类型 | JSON 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [获取用户详细信息](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | Stream           | 获取用户执行的 Yammer 活动的详细信息。                   |
| [获取活动数](../api/reportroot-getyammeractivitycounts.md) | Stream          | Stream           | 获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。 |
| [获取用户数](../api/reportroot-getyammeractivityusercounts.md) | Stream          | Stream           | 获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。 |


