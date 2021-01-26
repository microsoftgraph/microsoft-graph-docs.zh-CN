---
title: OneDrive 使用情况报表
description: OneDrive 使用情况报表可用于大致了解 OneDrive 带来的价值，具体是以跨组织中所有 OneDrive 帐户的文件总数和存储为依据。 然后，可以向下钻取活跃 OneDrive 帐户的趋势、用户已交互的文件数以及使用的存储空间。 这些报表还提供每个 OneDrive 帐户的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 22ed2e491bb8ed2631968d35490ca902fce93e4b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980988"
---
# <a name="onedrive-usage-reports"></a><span data-ttu-id="93cd8-105">OneDrive 使用情况报表</span><span class="sxs-lookup"><span data-stu-id="93cd8-105">OneDrive usage reports</span></span>

<span data-ttu-id="93cd8-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93cd8-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93cd8-107">OneDrive 使用情况报表可用于大致了解 OneDrive 带来的价值，具体是以跨组织中所有 OneDrive 帐户的文件总数和存储为依据。</span><span class="sxs-lookup"><span data-stu-id="93cd8-107">You can use the OneDrive usage reports to gain a high-level view of the value you are getting from OneDrive in terms of the total number of files and storage used across all the OneDrive accounts in your organization.</span></span> <span data-ttu-id="93cd8-108">然后，可以向下钻取活跃 OneDrive 帐户的趋势、用户已交互的文件数以及使用的存储空间。</span><span class="sxs-lookup"><span data-stu-id="93cd8-108">You can then drill down to understand the trends of active OneDrive accounts, how many files users have interacted with, and how much storage is used.</span></span> <span data-ttu-id="93cd8-109">这些报表还提供每个 OneDrive 帐户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="93cd8-109">These reports can also give you the details per OneDrive account.</span></span>

> <span data-ttu-id="93cd8-110">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="93cd8-110">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="reports"></a><span data-ttu-id="93cd8-111">报告</span><span class="sxs-lookup"><span data-stu-id="93cd8-111">Reports</span></span>

| <span data-ttu-id="93cd8-112">函数</span><span class="sxs-lookup"><span data-stu-id="93cd8-112">Function</span></span>                                 | <span data-ttu-id="93cd8-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="93cd8-113">Return Type</span></span> | <span data-ttu-id="93cd8-114">说明</span><span class="sxs-lookup"><span data-stu-id="93cd8-114">Description</span></span>                              |
| :--------------------------------------- | :---------- | ---------------------------------------- |
| [<span data-ttu-id="93cd8-115">获取帐户详细信息</span><span class="sxs-lookup"><span data-stu-id="93cd8-115">Get account detail</span></span>](../api/reportroot-getonedriveusageaccountdetail.md) | <span data-ttu-id="93cd8-116">Stream</span><span class="sxs-lookup"><span data-stu-id="93cd8-116">Stream</span></span>      | <span data-ttu-id="93cd8-117">获取帐户的 OneDrive 使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="93cd8-117">Get details about OneDrive usage by account.</span></span> |
| [<span data-ttu-id="93cd8-118">获取帐户数</span><span class="sxs-lookup"><span data-stu-id="93cd8-118">Get account counts</span></span>](../api/reportroot-getonedriveusageaccountcounts.md) | <span data-ttu-id="93cd8-119">Stream</span><span class="sxs-lookup"><span data-stu-id="93cd8-119">Stream</span></span>      | <span data-ttu-id="93cd8-120">获取 OneDrive for Business 活跃网站数趋势。</span><span class="sxs-lookup"><span data-stu-id="93cd8-120">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="93cd8-121">用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。</span><span class="sxs-lookup"><span data-stu-id="93cd8-121">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span> |
| [<span data-ttu-id="93cd8-122">获取文件数</span><span class="sxs-lookup"><span data-stu-id="93cd8-122">Get file counts</span></span>](../api/reportroot-getonedriveusagefilecounts.md) | <span data-ttu-id="93cd8-123">Stream</span><span class="sxs-lookup"><span data-stu-id="93cd8-123">Stream</span></span>      | <span data-ttu-id="93cd8-124">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="93cd8-124">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="93cd8-125">如果文件在指定时间段内被保存、同步、修改或共享，则视为活跃文件。</span><span class="sxs-lookup"><span data-stu-id="93cd8-125">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span> |
| [<span data-ttu-id="93cd8-126">获取存储</span><span class="sxs-lookup"><span data-stu-id="93cd8-126">Get storage</span></span>](../api/reportroot-getonedriveusagestorage.md) | <span data-ttu-id="93cd8-127">Stream</span><span class="sxs-lookup"><span data-stu-id="93cd8-127">Stream</span></span>      | <span data-ttu-id="93cd8-128">获取 OneDrive for Business 使用的存储空间趋势。</span><span class="sxs-lookup"><span data-stu-id="93cd8-128">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span> |

