---
title: 邮箱使用情况报表
description: 您可以通过邮箱和活动的主要基于电子邮件发送和接收其级别的用户的信息。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: a91e01edc3b2d61494a51b9bf53f1f0612a64343
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923122"
---
# <a name="mailbox-usage-reports"></a>邮箱使用情况报表

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

您可以通过邮箱和活动的主要基于电子邮件发送和接收其级别的用户的信息。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取邮箱详细信息](../api/reportroot-getmailboxusagedetail.md) | Stream          | [mailboxUsageDetail](../resources/mailboxusagedetail.md) | 获取邮箱使用情况的详细信息。         |
| [获取邮箱数](../api/reportroot-getmailboxusagemailboxcounts.md) | Stream          | [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) | 获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。 如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。 |
| [获取配额状态邮箱数](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Stream          | [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) | 获取每个配额类别中的用户邮箱数。 |
| [获取存储](../api/reportroot-getmailboxusagestorage.md) | Stream          | [mailboxUsageStorage](../resources/mailboxusagestorage.md) | 获取组织使用的存储空间。 |
