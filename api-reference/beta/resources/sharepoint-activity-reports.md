---
title: SharePoint 活动报表
description: 您可以通过查看用户与文件的交互来获取使用 SharePoint 的每个用户的活动。 也可以查看以共享文件数为依据的协作级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: b787fe2828519c6c21fa0c0b605ba9045c31ae84
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520722"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="21951-104">SharePoint 活动报表</span><span class="sxs-lookup"><span data-stu-id="21951-104">SharePoint activity reports</span></span>

<span data-ttu-id="21951-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="21951-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21951-106">您可以通过查看用户与文件的交互来获取使用 SharePoint 的每个用户的活动。</span><span class="sxs-lookup"><span data-stu-id="21951-106">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="21951-107">也可以查看以共享文件数为依据的协作级别。</span><span class="sxs-lookup"><span data-stu-id="21951-107">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="21951-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="21951-108">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="21951-109">报表</span><span class="sxs-lookup"><span data-stu-id="21951-109">Reports</span></span>

| <span data-ttu-id="21951-110">函数</span><span class="sxs-lookup"><span data-stu-id="21951-110">Function</span></span>                                 | <span data-ttu-id="21951-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="21951-111">CSV Return Type</span></span> | <span data-ttu-id="21951-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="21951-112">JSON Return Type</span></span>                         | <span data-ttu-id="21951-113">说明</span><span class="sxs-lookup"><span data-stu-id="21951-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="21951-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="21951-114">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="21951-115">Stream</span><span class="sxs-lookup"><span data-stu-id="21951-115">Stream</span></span>          | [<span data-ttu-id="21951-116">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="21951-116">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="21951-117">获取用户执行的 SharePoint 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="21951-117">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="21951-118">获取文件数</span><span class="sxs-lookup"><span data-stu-id="21951-118">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="21951-119">Stream</span><span class="sxs-lookup"><span data-stu-id="21951-119">Stream</span></span>          | [<span data-ttu-id="21951-120">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="21951-120">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="21951-121">获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="21951-121">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="21951-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="21951-122">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="21951-123">Stream</span><span class="sxs-lookup"><span data-stu-id="21951-123">Stream</span></span>          | [<span data-ttu-id="21951-124">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="21951-124">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="21951-125">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="21951-125">Get the trend in the number of active users.</span></span> <span data-ttu-id="21951-126">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="21951-126">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="21951-127">获取页面数</span><span class="sxs-lookup"><span data-stu-id="21951-127">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="21951-128">Stream</span><span class="sxs-lookup"><span data-stu-id="21951-128">Stream</span></span>          | [<span data-ttu-id="21951-129">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="21951-129">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="21951-130">获取用户访问的唯一页面数。</span><span class="sxs-lookup"><span data-stu-id="21951-130">Get the number of unique pages visited by users.</span></span> |
