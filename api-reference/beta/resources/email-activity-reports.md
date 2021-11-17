---
title: 电子邮件活动报表
description: You can get a high level view of email traffic within your organization from the Reports page. 您还可以深入了解"电子邮件活动"小部件，了解组织中电子邮件活动的每个用户的趋势和详细信息。
ms.localizationpriority: medium
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: d4599c3b0192289e8cd0e5c4d4aa59876aed075f
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044790"
---
# <a name="email-activity-reports"></a>电子邮件活动报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

You can get a high level view of email traffic within your organization from the Reports page. 您还可以深入了解"电子邮件活动"小部件，了解组织中电子邮件活动的每个用户的趋势和详细信息。

> **备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 邮箱活动况](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。

## <a name="reports"></a>报告

| 函数                                                     | CSV 返回类型 | JSON 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [获取用户详细信息](../api/reportroot-getemailactivityuserdetail.md) | Stream          | Stream           | 获取用户执行的电子邮件活动的详细信息。       |
| [获取活动数](../api/reportroot-getemailactivitycounts.md) | Stream          | Stream           | 可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。 |
| [获取用户数](../api/reportroot-getemailactivityusercounts.md) | Stream          | Stream           | 可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。 |


