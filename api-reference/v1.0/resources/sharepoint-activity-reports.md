---
title: SharePoint 活动报表
description: SharePoint 活动报表可用于获取每个有权使用 SharePoint 的用户的活动，具体是以用户与文件的交互为依据。 也可以查看以共享文件数为依据的协作级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 7d0e323c81ed421c2234bbd78bb3d98a9f21c8bb
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895991"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="2ed99-104">SharePoint 活动报表</span><span class="sxs-lookup"><span data-stu-id="2ed99-104">SharePoint activity reports</span></span>

<span data-ttu-id="2ed99-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ed99-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ed99-106">SharePoint 活动报表可用于获取每个有权使用 SharePoint 的用户的活动，具体是以用户与文件的交互为依据。</span><span class="sxs-lookup"><span data-stu-id="2ed99-106">You can use the SharePoint activity reports to get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="2ed99-107">也可以查看以共享文件数为依据的协作级别。</span><span class="sxs-lookup"><span data-stu-id="2ed99-107">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="2ed99-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="2ed99-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="2ed99-109">报表</span><span class="sxs-lookup"><span data-stu-id="2ed99-109">Reports</span></span>

| <span data-ttu-id="2ed99-110">函数</span><span class="sxs-lookup"><span data-stu-id="2ed99-110">Function</span></span>                                 | <span data-ttu-id="2ed99-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="2ed99-111">Return Type</span></span> | <span data-ttu-id="2ed99-112">说明</span><span class="sxs-lookup"><span data-stu-id="2ed99-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="2ed99-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="2ed99-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="2ed99-114">Stream</span><span class="sxs-lookup"><span data-stu-id="2ed99-114">Stream</span></span>      | <span data-ttu-id="2ed99-115">获取用户执行的 SharePoint 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2ed99-115">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="2ed99-116">获取文件数</span><span class="sxs-lookup"><span data-stu-id="2ed99-116">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="2ed99-117">Stream</span><span class="sxs-lookup"><span data-stu-id="2ed99-117">Stream</span></span>      | <span data-ttu-id="2ed99-118">获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="2ed99-118">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="2ed99-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="2ed99-119">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="2ed99-120">Stream</span><span class="sxs-lookup"><span data-stu-id="2ed99-120">Stream</span></span>      | <span data-ttu-id="2ed99-121">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="2ed99-121">Get the trend in the number of active users.</span></span> <span data-ttu-id="2ed99-122">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="2ed99-122">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="2ed99-123">获取页面数</span><span class="sxs-lookup"><span data-stu-id="2ed99-123">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="2ed99-124">Stream</span><span class="sxs-lookup"><span data-stu-id="2ed99-124">Stream</span></span>      | <span data-ttu-id="2ed99-125">获取用户访问的唯一页面数。</span><span class="sxs-lookup"><span data-stu-id="2ed99-125">Get the number of unique pages visited by users.</span></span> |
