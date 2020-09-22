---
title: 邮箱使用情况报表
description: 您可以使用邮箱及其活动级别（主要基于发送和接收的电子邮件）获取有关用户的信息。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: f3942bc4dc0eebb66a8ec0b9a8fc08619089c264
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095017"
---
# <a name="mailbox-usage-reports"></a>邮箱使用情况报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以使用邮箱及其活动级别（主要基于发送和接收的电子邮件）获取有关用户的信息。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表-邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取邮箱详细信息](../api/reportroot-getmailboxusagedetail.md) | Stream          | [mailboxUsageDetail](../resources/mailboxusagedetail.md) | 获取邮箱使用情况的详细信息。         |
| [获取邮箱数](../api/reportroot-getmailboxusagemailboxcounts.md) | Stream          | [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) | 获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。 如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。 |
| [获取配额状态邮箱数](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Stream          | [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) | 获取每个配额类别中的用户邮箱数。 |
| [获取存储](../api/reportroot-getmailboxusagestorage.md) | Stream          | [mailboxUsageStorage](../resources/mailboxusagestorage.md) | 获取组织使用的存储空间。 |


