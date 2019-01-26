---
title: 邮箱使用情况报表
description: 您可以通过邮箱和活动的主要基于电子邮件发送和接收其级别的用户的信息。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: ae0b3294750271f32d91dca79f75e7cf44641045
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576323"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="70fa9-104">邮箱使用情况报表</span><span class="sxs-lookup"><span data-stu-id="70fa9-104">Mailbox usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70fa9-105">您可以通过邮箱和活动的主要基于电子邮件发送和接收其级别的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="70fa9-105">You can get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="70fa9-106">此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。</span><span class="sxs-lookup"><span data-stu-id="70fa9-106">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="70fa9-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="70fa9-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="70fa9-108">报表</span><span class="sxs-lookup"><span data-stu-id="70fa9-108">Reports</span></span>

| <span data-ttu-id="70fa9-109">函数</span><span class="sxs-lookup"><span data-stu-id="70fa9-109">Function</span></span>                                 | <span data-ttu-id="70fa9-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="70fa9-110">CSV return type</span></span> | <span data-ttu-id="70fa9-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="70fa9-111">JSON return type</span></span>                         | <span data-ttu-id="70fa9-112">说明</span><span class="sxs-lookup"><span data-stu-id="70fa9-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="70fa9-113">获取邮箱详细信息</span><span class="sxs-lookup"><span data-stu-id="70fa9-113">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="70fa9-114">Stream</span><span class="sxs-lookup"><span data-stu-id="70fa9-114">Stream</span></span>          | [<span data-ttu-id="70fa9-115">mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="70fa9-115">mailboxUsageDetail</span></span>](../resources/mailboxusagedetail.md) | <span data-ttu-id="70fa9-116">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="70fa9-116">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="70fa9-117">获取邮箱数</span><span class="sxs-lookup"><span data-stu-id="70fa9-117">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="70fa9-118">Stream</span><span class="sxs-lookup"><span data-stu-id="70fa9-118">Stream</span></span>          | [<span data-ttu-id="70fa9-119">mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="70fa9-119">mailboxUsageMailboxCounts</span></span>](../resources/mailboxusagemailboxcounts.md) | <span data-ttu-id="70fa9-120">获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。</span><span class="sxs-lookup"><span data-stu-id="70fa9-120">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="70fa9-121">如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。</span><span class="sxs-lookup"><span data-stu-id="70fa9-121">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="70fa9-122">获取配额状态邮箱数</span><span class="sxs-lookup"><span data-stu-id="70fa9-122">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="70fa9-123">Stream</span><span class="sxs-lookup"><span data-stu-id="70fa9-123">Stream</span></span>          | [<span data-ttu-id="70fa9-124">mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="70fa9-124">mailboxUsageQuotaStatusMailboxCounts</span></span>](../resources/mailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="70fa9-125">获取每个配额类别中的用户邮箱数。</span><span class="sxs-lookup"><span data-stu-id="70fa9-125">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="70fa9-126">获取存储</span><span class="sxs-lookup"><span data-stu-id="70fa9-126">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="70fa9-127">Stream</span><span class="sxs-lookup"><span data-stu-id="70fa9-127">Stream</span></span>          | [<span data-ttu-id="70fa9-128">mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="70fa9-128">mailboxUsageStorage</span></span>](../resources/mailboxusagestorage.md) | <span data-ttu-id="70fa9-129">获取组织使用的存储空间。</span><span class="sxs-lookup"><span data-stu-id="70fa9-129">Get the amount of storage used in your organization.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailbox-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
