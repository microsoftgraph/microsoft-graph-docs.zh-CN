---
title: 电子邮件活动报表
description: 电子邮件活动报表可用于大致了解组织中的电子邮件流量。 此外，还可以向下钻取“电子邮件活动”小组件，了解组织中每个用户的电子邮件活动的趋势和详细信息。
localization_priority: Priority
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 110502c61a25ae046aa17fde72a5ffc64368b1eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531487"
---
# <a name="email-activity-reports"></a>电子邮件活动报告

命名空间：microsoft.graph

电子邮件活动报表可用于大致了解组织中的电子邮件流量。 此外，还可以向下钻取“电子邮件活动”小组件，了解组织中每个用户的电子邮件活动的趋势和详细信息。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getemailactivityuserdetail.md) | Stream      | 获取用户执行的电子邮件活动的详细信息。 |
| [获取活动数](../api/reportroot-getemailactivitycounts.md) | Stream      | 可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。 |
| [获取用户数](../api/reportroot-getemailactivityusercounts.md) | Stream      | 可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。 |
