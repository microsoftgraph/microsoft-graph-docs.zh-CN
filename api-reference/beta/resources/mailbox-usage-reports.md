---
title: 邮箱使用情况报表
description: 您可以获取有关具有邮箱的用户及其活动级别的信息，这些信息主要基于已发送和接收的电子邮件。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: c679e8b73e0e2a43ded3bffd66fe7c9d14a957d1
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983564"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="523cf-104">邮箱使用情况报表</span><span class="sxs-lookup"><span data-stu-id="523cf-104">Mailbox usage reports</span></span>

<span data-ttu-id="523cf-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="523cf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="523cf-106">您可以获取有关具有邮箱的用户及其活动级别的信息，这些信息主要基于已发送和接收的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="523cf-106">You can get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="523cf-107">此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。</span><span class="sxs-lookup"><span data-stu-id="523cf-107">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="523cf-108">**备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="523cf-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="523cf-109">报告</span><span class="sxs-lookup"><span data-stu-id="523cf-109">Reports</span></span>

| <span data-ttu-id="523cf-110">函数</span><span class="sxs-lookup"><span data-stu-id="523cf-110">Function</span></span>                                 | <span data-ttu-id="523cf-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="523cf-111">CSV return type</span></span> | <span data-ttu-id="523cf-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="523cf-112">JSON return type</span></span>                         | <span data-ttu-id="523cf-113">说明</span><span class="sxs-lookup"><span data-stu-id="523cf-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="523cf-114">获取邮箱详细信息</span><span class="sxs-lookup"><span data-stu-id="523cf-114">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="523cf-115">Stream</span><span class="sxs-lookup"><span data-stu-id="523cf-115">Stream</span></span>          | [<span data-ttu-id="523cf-116">mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="523cf-116">mailboxUsageDetail</span></span>](../resources/mailboxusagedetail.md) | <span data-ttu-id="523cf-117">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="523cf-117">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="523cf-118">获取邮箱数</span><span class="sxs-lookup"><span data-stu-id="523cf-118">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="523cf-119">Stream</span><span class="sxs-lookup"><span data-stu-id="523cf-119">Stream</span></span>          | [<span data-ttu-id="523cf-120">mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="523cf-120">mailboxUsageMailboxCounts</span></span>](../resources/mailboxusagemailboxcounts.md) | <span data-ttu-id="523cf-121">获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。</span><span class="sxs-lookup"><span data-stu-id="523cf-121">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="523cf-122">如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。</span><span class="sxs-lookup"><span data-stu-id="523cf-122">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="523cf-123">获取配额状态邮箱数</span><span class="sxs-lookup"><span data-stu-id="523cf-123">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="523cf-124">Stream</span><span class="sxs-lookup"><span data-stu-id="523cf-124">Stream</span></span>          | [<span data-ttu-id="523cf-125">mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="523cf-125">mailboxUsageQuotaStatusMailboxCounts</span></span>](../resources/mailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="523cf-126">获取每个配额类别中的用户邮箱数。</span><span class="sxs-lookup"><span data-stu-id="523cf-126">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="523cf-127">获取存储</span><span class="sxs-lookup"><span data-stu-id="523cf-127">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="523cf-128">Stream</span><span class="sxs-lookup"><span data-stu-id="523cf-128">Stream</span></span>          | [<span data-ttu-id="523cf-129">mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="523cf-129">mailboxUsageStorage</span></span>](../resources/mailboxusagestorage.md) | <span data-ttu-id="523cf-130">获取组织使用的存储空间。</span><span class="sxs-lookup"><span data-stu-id="523cf-130">Get the amount of storage used in your organization.</span></span> |


