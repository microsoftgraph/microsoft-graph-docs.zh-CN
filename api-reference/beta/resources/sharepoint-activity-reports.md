---
title: SharePoint 活动报表
description: 您可以通过查看用户与文件的交互来获取使用 SharePoint 的每个用户的活动。 也可以查看以共享文件数为依据的协作级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: cf2aad8f76eebefc013f293c9b90c93793c3d463
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895557"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="fb95e-104">SharePoint 活动报表</span><span class="sxs-lookup"><span data-stu-id="fb95e-104">SharePoint activity reports</span></span>

<span data-ttu-id="fb95e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb95e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb95e-106">您可以通过查看用户与文件的交互来获取使用 SharePoint 的每个用户的活动。</span><span class="sxs-lookup"><span data-stu-id="fb95e-106">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="fb95e-107">也可以查看以共享文件数为依据的协作级别。</span><span class="sxs-lookup"><span data-stu-id="fb95e-107">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="fb95e-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="fb95e-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="fb95e-109">报表</span><span class="sxs-lookup"><span data-stu-id="fb95e-109">Reports</span></span>

| <span data-ttu-id="fb95e-110">函数</span><span class="sxs-lookup"><span data-stu-id="fb95e-110">Function</span></span>                                 | <span data-ttu-id="fb95e-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="fb95e-111">CSV Return Type</span></span> | <span data-ttu-id="fb95e-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="fb95e-112">JSON Return Type</span></span>                         | <span data-ttu-id="fb95e-113">说明</span><span class="sxs-lookup"><span data-stu-id="fb95e-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="fb95e-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="fb95e-114">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="fb95e-115">Stream</span><span class="sxs-lookup"><span data-stu-id="fb95e-115">Stream</span></span>          | [<span data-ttu-id="fb95e-116">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="fb95e-116">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="fb95e-117">获取用户执行的 SharePoint 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fb95e-117">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="fb95e-118">获取文件数</span><span class="sxs-lookup"><span data-stu-id="fb95e-118">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="fb95e-119">Stream</span><span class="sxs-lookup"><span data-stu-id="fb95e-119">Stream</span></span>          | [<span data-ttu-id="fb95e-120">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="fb95e-120">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="fb95e-121">获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="fb95e-121">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="fb95e-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="fb95e-122">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="fb95e-123">Stream</span><span class="sxs-lookup"><span data-stu-id="fb95e-123">Stream</span></span>          | [<span data-ttu-id="fb95e-124">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="fb95e-124">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="fb95e-125">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="fb95e-125">Get the trend in the number of active users.</span></span> <span data-ttu-id="fb95e-126">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="fb95e-126">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="fb95e-127">获取页面数</span><span class="sxs-lookup"><span data-stu-id="fb95e-127">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="fb95e-128">Stream</span><span class="sxs-lookup"><span data-stu-id="fb95e-128">Stream</span></span>          | [<span data-ttu-id="fb95e-129">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="fb95e-129">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="fb95e-130">获取用户访问的唯一页面数。</span><span class="sxs-lookup"><span data-stu-id="fb95e-130">Get the number of unique pages visited by users.</span></span> |
