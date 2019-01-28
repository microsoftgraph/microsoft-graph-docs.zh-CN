---
title: 邮箱使用情况报表
description: 邮箱使用情况报表可用于获取使用邮箱的用户及其活动级别（主要是以发送和接收的电子邮件数为依据）。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。
localization_priority: Priority
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 6b02821da78338e8af1dec99fe73bedf81561116
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574647"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="43b4f-104">邮箱使用情况报告</span><span class="sxs-lookup"><span data-stu-id="43b4f-104">Mailbox usage reports</span></span>

<span data-ttu-id="43b4f-105">邮箱使用情况报表可用于获取使用邮箱的用户及其活动级别（主要是以发送和接收的电子邮件数为依据）。</span><span class="sxs-lookup"><span data-stu-id="43b4f-105">Use the mailbox usage reports to get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="43b4f-106">此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。</span><span class="sxs-lookup"><span data-stu-id="43b4f-106">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="43b4f-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="43b4f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="43b4f-108">报表</span><span class="sxs-lookup"><span data-stu-id="43b4f-108">Reports</span></span>

| <span data-ttu-id="43b4f-109">函数</span><span class="sxs-lookup"><span data-stu-id="43b4f-109">Function</span></span>                                 | <span data-ttu-id="43b4f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="43b4f-110">Return Type</span></span> | <span data-ttu-id="43b4f-111">说明</span><span class="sxs-lookup"><span data-stu-id="43b4f-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="43b4f-112">获取邮箱详细信息</span><span class="sxs-lookup"><span data-stu-id="43b4f-112">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="43b4f-113">Stream</span><span class="sxs-lookup"><span data-stu-id="43b4f-113">Stream</span></span>      | <span data-ttu-id="43b4f-114">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="43b4f-114">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="43b4f-115">获取邮箱数</span><span class="sxs-lookup"><span data-stu-id="43b4f-115">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="43b4f-116">Stream</span><span class="sxs-lookup"><span data-stu-id="43b4f-116">Stream</span></span>      | <span data-ttu-id="43b4f-117">获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。</span><span class="sxs-lookup"><span data-stu-id="43b4f-117">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="43b4f-118">如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。</span><span class="sxs-lookup"><span data-stu-id="43b4f-118">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="43b4f-119">获取配额状态邮箱数</span><span class="sxs-lookup"><span data-stu-id="43b4f-119">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="43b4f-120">Stream</span><span class="sxs-lookup"><span data-stu-id="43b4f-120">Stream</span></span>      | <span data-ttu-id="43b4f-121">获取每个配额类别中的用户邮箱数。</span><span class="sxs-lookup"><span data-stu-id="43b4f-121">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="43b4f-122">获取存储</span><span class="sxs-lookup"><span data-stu-id="43b4f-122">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="43b4f-123">Stream</span><span class="sxs-lookup"><span data-stu-id="43b4f-123">Stream</span></span>      | <span data-ttu-id="43b4f-124">获取组织使用的存储空间。</span><span class="sxs-lookup"><span data-stu-id="43b4f-124">Get the amount of storage used in your organization.</span></span> |
