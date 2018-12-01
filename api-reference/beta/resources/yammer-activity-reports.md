---
title: Yammer 活动报表
description: 您可以通过多少活动生成跨组织和发布、 like，和阅读 Yammer 上的消息的唯一用户数了解 Yammer 与贵组织的工作效率的级别。
ms.openlocfilehash: 3d70af700a55359044b4c24896a0118de5280fee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044617"
---
# <a name="yammer-activity-reports"></a>Yammer 活动报表

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。 在 Microsoft Graph 中国由 21Vianet 不支持这些 Api。

您可以通过多少活动生成跨组织和发布、 like，和阅读 Yammer 上的消息的唯一用户数了解 Yammer 与贵组织的工作效率的级别。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | 获取用户执行的 Yammer 活动的详细信息。 |
| [获取活动数](../api/reportroot-getyammeractivitycounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | 获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。 |
| [获取用户数](../api/reportroot-getyammeractivityusercounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | 获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。 |
