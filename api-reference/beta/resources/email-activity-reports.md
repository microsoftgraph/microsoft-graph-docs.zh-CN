---
title: 电子邮件活动报表
description: 您可以从 "报告" 页面获取组织中的电子邮件流量的高级视图。 您还可以深入了解电子邮件活动小组件，以了解组织中的电子邮件活动的每个用户的趋势和详细信息。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 5f26498a0837993fc052cb536acd8bcd08f77ee1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896908"
---
# <a name="email-activity-reports"></a>电子邮件活动报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以从 "报告" 页面获取组织中的电子邮件流量的高级视图。 您还可以深入了解电子邮件活动小组件，以了解组织中的电子邮件活动的每个用户的趋势和详细信息。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getemailactivityuserdetail.md) | Stream          | [emailActivityUserDetail](../resources/emailactivityuserdetail.md) | 获取用户执行的电子邮件活动的详细信息。 |
| [获取活动数](../api/reportroot-getemailactivitycounts.md) | Stream          | [emailActivitySummary](../resources/emailactivitysummary.md) | 可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。 |
| [获取用户数](../api/reportroot-getemailactivityusercounts.md) | Stream          | [emailActivitySummary](../resources/emailactivitysummary.md) | 可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。 |
