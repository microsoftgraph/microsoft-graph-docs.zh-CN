---
title: 邮箱使用情况报表
description: 您可以使用邮箱及其活动级别（主要基于发送和接收的电子邮件）获取有关用户的信息。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: c6e356ee1c6f8937f1c252c7dd8e8c20174ba86b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522874"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="851af-104">邮箱使用情况报告</span><span class="sxs-lookup"><span data-stu-id="851af-104">Mailbox usage reports</span></span>

<span data-ttu-id="851af-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="851af-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="851af-106">您可以使用邮箱及其活动级别（主要基于发送和接收的电子邮件）获取有关用户的信息。</span><span class="sxs-lookup"><span data-stu-id="851af-106">You can get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="851af-107">此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。</span><span class="sxs-lookup"><span data-stu-id="851af-107">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="851af-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="851af-108">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="851af-109">报表</span><span class="sxs-lookup"><span data-stu-id="851af-109">Reports</span></span>

| <span data-ttu-id="851af-110">函数</span><span class="sxs-lookup"><span data-stu-id="851af-110">Function</span></span>                                 | <span data-ttu-id="851af-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="851af-111">CSV return type</span></span> | <span data-ttu-id="851af-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="851af-112">JSON return type</span></span>                         | <span data-ttu-id="851af-113">说明</span><span class="sxs-lookup"><span data-stu-id="851af-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="851af-114">获取邮箱详细信息</span><span class="sxs-lookup"><span data-stu-id="851af-114">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="851af-115">Stream</span><span class="sxs-lookup"><span data-stu-id="851af-115">Stream</span></span>          | [<span data-ttu-id="851af-116">mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="851af-116">mailboxUsageDetail</span></span>](../resources/mailboxusagedetail.md) | <span data-ttu-id="851af-117">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="851af-117">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="851af-118">获取邮箱数</span><span class="sxs-lookup"><span data-stu-id="851af-118">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="851af-119">Stream</span><span class="sxs-lookup"><span data-stu-id="851af-119">Stream</span></span>          | [<span data-ttu-id="851af-120">mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="851af-120">mailboxUsageMailboxCounts</span></span>](../resources/mailboxusagemailboxcounts.md) | <span data-ttu-id="851af-121">获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。</span><span class="sxs-lookup"><span data-stu-id="851af-121">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="851af-122">如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。</span><span class="sxs-lookup"><span data-stu-id="851af-122">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="851af-123">获取配额状态邮箱数</span><span class="sxs-lookup"><span data-stu-id="851af-123">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="851af-124">Stream</span><span class="sxs-lookup"><span data-stu-id="851af-124">Stream</span></span>          | [<span data-ttu-id="851af-125">mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="851af-125">mailboxUsageQuotaStatusMailboxCounts</span></span>](../resources/mailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="851af-126">获取每个配额类别中的用户邮箱数。</span><span class="sxs-lookup"><span data-stu-id="851af-126">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="851af-127">获取存储</span><span class="sxs-lookup"><span data-stu-id="851af-127">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="851af-128">Stream</span><span class="sxs-lookup"><span data-stu-id="851af-128">Stream</span></span>          | [<span data-ttu-id="851af-129">mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="851af-129">mailboxUsageStorage</span></span>](../resources/mailboxusagestorage.md) | <span data-ttu-id="851af-130">获取组织使用的存储空间。</span><span class="sxs-lookup"><span data-stu-id="851af-130">Get the amount of storage used in your organization.</span></span> |
