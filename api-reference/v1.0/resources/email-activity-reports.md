---
title: 电子邮件活动报表
description: 电子邮件活动报表可用于大致了解组织中的电子邮件流量。 此外，还可以向下钻取“电子邮件活动”小组件，了解组织中每个用户的电子邮件活动的趋势和详细信息。
localization_priority: Priority
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 7f0716d42d9b3e2f2fa360e065ebfd9ed7e1a4fc
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982941"
---
# <a name="email-activity-reports"></a>电子邮件活动报告

命名空间：microsoft.graph

电子邮件活动报表可用于大致了解组织中的电子邮件流量。 此外，还可以向下钻取“电子邮件活动”小组件，了解组织中每个用户的电子邮件活动的趋势和详细信息。

> **备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 邮箱活动况](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。

## <a name="reports"></a>报告

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getemailactivityuserdetail.md) | Stream      | 获取用户执行的电子邮件活动的详细信息。 |
| [获取活动数](../api/reportroot-getemailactivitycounts.md) | Stream      | 可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。 |
| [获取用户数](../api/reportroot-getemailactivityusercounts.md) | Stream      | 可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。 |

