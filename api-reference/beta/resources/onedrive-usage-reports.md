---
title: OneDrive 使用情况报表
description: 您可以从在组织的所有 OneDrive 帐户中使用的文件总数和存储量中获取您从 OneDrive 获取的值的高级视图。 然后，可以向下钻取活跃 OneDrive 帐户的趋势、用户已交互的文件数以及使用的存储空间。 它还提供了每个 OneDrive 帐户的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1f899c3a60e1c0d66dd3b7e075bf0daf13de0b43
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457086"
---
# <a name="onedrive-usage-reports"></a><span data-ttu-id="03691-105">OneDrive 使用情况报表</span><span class="sxs-lookup"><span data-stu-id="03691-105">OneDrive usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03691-106">您可以从在组织的所有 OneDrive 帐户中使用的文件总数和存储量中获取您从 OneDrive 获取的值的高级视图。</span><span class="sxs-lookup"><span data-stu-id="03691-106">You can get a high-level view of the value you are getting from OneDrive in terms of the total number of files and storage used across all the OneDrive accounts in your organization.</span></span> <span data-ttu-id="03691-107">然后，可以向下钻取活跃 OneDrive 帐户的趋势、用户已交互的文件数以及使用的存储空间。</span><span class="sxs-lookup"><span data-stu-id="03691-107">You can then drill down to understand the trends of active OneDrive accounts, how many files users have interacted with, and how much storage is used.</span></span> <span data-ttu-id="03691-108">它还提供了每个 OneDrive 帐户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="03691-108">It also gives you the per OneDrive account details.</span></span>

> <span data-ttu-id="03691-109">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="03691-109">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="reports"></a><span data-ttu-id="03691-110">报表</span><span class="sxs-lookup"><span data-stu-id="03691-110">Reports</span></span>

| <span data-ttu-id="03691-111">函数</span><span class="sxs-lookup"><span data-stu-id="03691-111">Function</span></span>                                 | <span data-ttu-id="03691-112">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="03691-112">CSV return type</span></span> | <span data-ttu-id="03691-113">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="03691-113">JSON return type</span></span>                         | <span data-ttu-id="03691-114">说明</span><span class="sxs-lookup"><span data-stu-id="03691-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | ---------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="03691-115">获取帐户详细信息</span><span class="sxs-lookup"><span data-stu-id="03691-115">Get account detail</span></span>](../api/reportroot-getonedriveusageaccountdetail.md) | <span data-ttu-id="03691-116">Stream</span><span class="sxs-lookup"><span data-stu-id="03691-116">Stream</span></span>          | [<span data-ttu-id="03691-117">oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="03691-117">oneDriveUsageAccountDetail</span></span>](../resources/onedriveusageaccountdetail.md) | <span data-ttu-id="03691-118">获取帐户的 OneDrive 使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="03691-118">Get details about OneDrive usage by account.</span></span> |
| [<span data-ttu-id="03691-119">获取帐户数</span><span class="sxs-lookup"><span data-stu-id="03691-119">Get account counts</span></span>](../api/reportroot-getonedriveusageaccountcounts.md) | <span data-ttu-id="03691-120">Stream</span><span class="sxs-lookup"><span data-stu-id="03691-120">Stream</span></span>          | [<span data-ttu-id="03691-121">oneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="03691-121">oneDriveUsageAccountCounts</span></span>](../resources/onedriveusageaccountcounts.md) | <span data-ttu-id="03691-122">获取 OneDrive for Business 活跃网站数趋势。</span><span class="sxs-lookup"><span data-stu-id="03691-122">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="03691-123">用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。</span><span class="sxs-lookup"><span data-stu-id="03691-123">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span> |
| [<span data-ttu-id="03691-124">获取文件数</span><span class="sxs-lookup"><span data-stu-id="03691-124">Get file counts</span></span>](../api/reportroot-getonedriveusagefilecounts.md) | <span data-ttu-id="03691-125">Stream</span><span class="sxs-lookup"><span data-stu-id="03691-125">Stream</span></span>          | [<span data-ttu-id="03691-126">oneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="03691-126">oneDriveUsageFileCounts</span></span>](../resources/onedriveusagefilecounts.md) | <span data-ttu-id="03691-127">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="03691-127">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="03691-128">如果文件在指定时间段内被保存、同步、修改或共享，则视为活跃文件。</span><span class="sxs-lookup"><span data-stu-id="03691-128">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span> |
| [<span data-ttu-id="03691-129">获取存储</span><span class="sxs-lookup"><span data-stu-id="03691-129">Get storage</span></span>](../api/reportroot-getonedriveusagestorage.md) | <span data-ttu-id="03691-130">Stream</span><span class="sxs-lookup"><span data-stu-id="03691-130">Stream</span></span>          | [<span data-ttu-id="03691-131">siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="03691-131">siteUsageStorage</span></span>](../resources/siteusagestorage.md) | <span data-ttu-id="03691-132">获取 OneDrive for Business 使用的存储空间趋势。</span><span class="sxs-lookup"><span data-stu-id="03691-132">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
