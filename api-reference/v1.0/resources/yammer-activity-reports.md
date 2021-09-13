---
title: Yammer 活动报表
description: Yammer 活动报表可用于了解组织的 Yammer 交互级别，具体是以整个组织中生成的活动数以及在 Yammer 上发布、赞和阅读消息的唯一用户数为依据。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 73204077e6e1b529c95e6f04a92291fe5229ef9c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59083906"
---
# <a name="yammer-activity-reports"></a>Yammer 活动报告

命名空间：microsoft.graph

Yammer 活动报表可用于了解组织的 Yammer 交互级别，具体是以整个组织中生成的活动数以及在 Yammer 上发布、赞和阅读消息的唯一用户数为依据。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅 Microsoft 365 [reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getyammeractivityuserdetail.md) | Stream      | 获取用户执行的 Yammer 活动的详细信息。 |
| [获取活动数](../api/reportroot-getyammeractivitycounts.md) | Stream      | 获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。 |
| [获取用户数](../api/reportroot-getyammeractivityusercounts.md) | Stream      | 获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。 |

