---
title: 电子邮件活动报表
description: 您可以从报告页的贵组织中获取电子邮件通信的高级视图。 您还可以钻取活动电子邮件小部件，以了解趋势和每个用户的组织中的电子邮件活动的详细信息。
ms.openlocfilehash: 47ff9017216fa3fd333b383f7a603354775d1023
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049390"
---
# <a name="email-activity-reports"></a>电子邮件活动报表

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

您可以从报告页的贵组织中获取电子邮件通信的高级视图。 您还可以钻取活动电子邮件小部件，以了解趋势和每个用户的组织中的电子邮件活动的详细信息。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getemailactivityuserdetail.md) | Stream          | [emailActivityUserDetail](../resources/emailactivityuserdetail.md) | 获取用户执行的电子邮件活动的详细信息。 |
| [获取活动数](../api/reportroot-getemailactivitycounts.md) | Stream          | [emailActivitySummary](../resources/emailactivitysummary.md) | 可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。 |
| [获取用户数](../api/reportroot-getemailactivityusercounts.md) | Stream          | [emailActivitySummary](../resources/emailactivitysummary.md) | 可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。 |
