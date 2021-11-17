---
title: 邮箱使用情况报表
description: 您可以获取有关具有邮箱的用户及其活动级别的信息，这些信息主要基于已发送和已接收的电子邮件。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。
ms.localizationpriority: medium
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: a6645a6952c2fe21cc2e7e323dccb61cc43e36b2
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044748"
---
# <a name="mailbox-usage-reports"></a>邮箱使用情况报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以获取有关具有邮箱的用户及其活动级别的信息，这些信息主要基于已发送和已接收的电子邮件。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。

> **备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。

## <a name="reports"></a>报告

| 函数                                                     | CSV 返回类型 | JSON 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [获取邮箱详细信息](../api/reportroot-getmailboxusagedetail.md) | Stream          | Stream           | 获取邮箱使用情况的详细信息。                             |
| [获取邮箱数](../api/reportroot-getmailboxusagemailboxcounts.md) | Stream          | Stream           | 获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。 如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。 |
| [获取配额状态邮箱数](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Stream          | Stream           | 获取每个配额类别中的用户邮箱数。      |
| [获取存储](../api/reportroot-getmailboxusagestorage.md)   | Stream          | Stream           | 获取组织使用的存储空间。         |


