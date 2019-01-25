---
title: Yammer 活动报表
description: 您可以通过多少活动生成跨组织和发布、 like，和阅读 Yammer 上的消息的唯一用户数了解 Yammer 与贵组织的工作效率的级别。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 252748b639f256467b2a01336488e1df086c69cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509936"
---
# <a name="yammer-activity-reports"></a>Yammer 活动报表

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以通过多少活动生成跨组织和发布、 like，和阅读 Yammer 上的消息的唯一用户数了解 Yammer 与贵组织的工作效率的级别。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | 获取用户执行的 Yammer 活动的详细信息。 |
| [获取活动数](../api/reportroot-getyammeractivitycounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | 获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。 |
| [获取用户数](../api/reportroot-getyammeractivityusercounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | 获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
