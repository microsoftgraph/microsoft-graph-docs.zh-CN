---
title: 邮箱使用情况报表
description: 邮箱使用情况报表可用于获取使用邮箱的用户及其活动级别（主要是以发送和接收的电子邮件数为依据）。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。
localization_priority: Priority
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: d460f2c72878065abdd1df2fa58dc0eb8f4d411b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981114"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="99e87-104">邮箱使用情况报表</span><span class="sxs-lookup"><span data-stu-id="99e87-104">Mailbox usage reports</span></span>

<span data-ttu-id="99e87-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99e87-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99e87-106">邮箱使用情况报表可用于获取使用邮箱的用户及其活动级别（主要是以发送和接收的电子邮件数为依据）。</span><span class="sxs-lookup"><span data-stu-id="99e87-106">Use the mailbox usage reports to get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="99e87-107">此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。</span><span class="sxs-lookup"><span data-stu-id="99e87-107">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="99e87-108">**备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="99e87-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="99e87-109">报告</span><span class="sxs-lookup"><span data-stu-id="99e87-109">Reports</span></span>

| <span data-ttu-id="99e87-110">函数</span><span class="sxs-lookup"><span data-stu-id="99e87-110">Function</span></span>                                 | <span data-ttu-id="99e87-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="99e87-111">Return Type</span></span> | <span data-ttu-id="99e87-112">说明</span><span class="sxs-lookup"><span data-stu-id="99e87-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="99e87-113">获取邮箱详细信息</span><span class="sxs-lookup"><span data-stu-id="99e87-113">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="99e87-114">Stream</span><span class="sxs-lookup"><span data-stu-id="99e87-114">Stream</span></span>      | <span data-ttu-id="99e87-115">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="99e87-115">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="99e87-116">获取邮箱数</span><span class="sxs-lookup"><span data-stu-id="99e87-116">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="99e87-117">Stream</span><span class="sxs-lookup"><span data-stu-id="99e87-117">Stream</span></span>      | <span data-ttu-id="99e87-118">获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。</span><span class="sxs-lookup"><span data-stu-id="99e87-118">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="99e87-119">如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。</span><span class="sxs-lookup"><span data-stu-id="99e87-119">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="99e87-120">获取配额状态邮箱数</span><span class="sxs-lookup"><span data-stu-id="99e87-120">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="99e87-121">Stream</span><span class="sxs-lookup"><span data-stu-id="99e87-121">Stream</span></span>      | <span data-ttu-id="99e87-122">获取每个配额类别中的用户邮箱数。</span><span class="sxs-lookup"><span data-stu-id="99e87-122">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="99e87-123">获取存储</span><span class="sxs-lookup"><span data-stu-id="99e87-123">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="99e87-124">Stream</span><span class="sxs-lookup"><span data-stu-id="99e87-124">Stream</span></span>      | <span data-ttu-id="99e87-125">获取组织使用的存储空间。</span><span class="sxs-lookup"><span data-stu-id="99e87-125">Get the amount of storage used in your organization.</span></span> |

