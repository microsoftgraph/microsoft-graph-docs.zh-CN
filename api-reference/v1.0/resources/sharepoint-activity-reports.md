---
title: SharePoint 活动报表
description: SharePoint 活动报表可用于获取每个有权使用 SharePoint 的用户的活动，具体是以用户与文件的交互为依据。 也可以查看以共享文件数为依据的协作级别。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 5d43f2183c805a29c0bb7a4693a01e14236537d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971891"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="e5569-104">SharePoint 活动报表</span><span class="sxs-lookup"><span data-stu-id="e5569-104">SharePoint activity reports</span></span>

<span data-ttu-id="e5569-105">SharePoint 活动报表可用于获取每个有权使用 SharePoint 的用户的活动，具体是以用户与文件的交互为依据。</span><span class="sxs-lookup"><span data-stu-id="e5569-105">You can use the SharePoint activity reports to get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="e5569-106">也可以查看以共享文件数为依据的协作级别。</span><span class="sxs-lookup"><span data-stu-id="e5569-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="e5569-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="e5569-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="e5569-108">报表</span><span class="sxs-lookup"><span data-stu-id="e5569-108">Reports</span></span>

| <span data-ttu-id="e5569-109">函数</span><span class="sxs-lookup"><span data-stu-id="e5569-109">Function</span></span>                                 | <span data-ttu-id="e5569-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5569-110">Return Type</span></span> | <span data-ttu-id="e5569-111">说明</span><span class="sxs-lookup"><span data-stu-id="e5569-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="e5569-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="e5569-112">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="e5569-113">Stream</span><span class="sxs-lookup"><span data-stu-id="e5569-113">Stream</span></span>      | <span data-ttu-id="e5569-114">获取用户执行的 SharePoint 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e5569-114">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="e5569-115">获取文件数</span><span class="sxs-lookup"><span data-stu-id="e5569-115">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="e5569-116">Stream</span><span class="sxs-lookup"><span data-stu-id="e5569-116">Stream</span></span>      | <span data-ttu-id="e5569-117">获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="e5569-117">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="e5569-118">获取用户数</span><span class="sxs-lookup"><span data-stu-id="e5569-118">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="e5569-119">Stream</span><span class="sxs-lookup"><span data-stu-id="e5569-119">Stream</span></span>      | <span data-ttu-id="e5569-120">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="e5569-120">Get the trend in the number of active users.</span></span> <span data-ttu-id="e5569-121">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="e5569-121">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="e5569-122">获取页面数</span><span class="sxs-lookup"><span data-stu-id="e5569-122">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="e5569-123">Stream</span><span class="sxs-lookup"><span data-stu-id="e5569-123">Stream</span></span>      | <span data-ttu-id="e5569-124">获取用户访问的唯一页面数。</span><span class="sxs-lookup"><span data-stu-id="e5569-124">Get the number of unique pages visited by users.</span></span> |
