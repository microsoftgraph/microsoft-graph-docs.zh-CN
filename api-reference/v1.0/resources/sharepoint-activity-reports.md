---
title: SharePoint 活动报表
description: SharePoint 活动报表可用于获取每个有权使用 SharePoint 的用户的活动，具体是以用户与文件的交互为依据。 也可以查看以共享文件数为依据的协作级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5754149f573798bfbb10a6ac6c2b9ca60fce597a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549606"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="40d5c-104">SharePoint 活动报表</span><span class="sxs-lookup"><span data-stu-id="40d5c-104">SharePoint activity reports</span></span>

<span data-ttu-id="40d5c-105">SharePoint 活动报表可用于获取每个有权使用 SharePoint 的用户的活动，具体是以用户与文件的交互为依据。</span><span class="sxs-lookup"><span data-stu-id="40d5c-105">You can use the SharePoint activity reports to get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="40d5c-106">也可以查看以共享文件数为依据的协作级别。</span><span class="sxs-lookup"><span data-stu-id="40d5c-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="40d5c-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="40d5c-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="40d5c-108">报表</span><span class="sxs-lookup"><span data-stu-id="40d5c-108">Reports</span></span>

| <span data-ttu-id="40d5c-109">函数</span><span class="sxs-lookup"><span data-stu-id="40d5c-109">Function</span></span>                                 | <span data-ttu-id="40d5c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="40d5c-110">Return Type</span></span> | <span data-ttu-id="40d5c-111">说明</span><span class="sxs-lookup"><span data-stu-id="40d5c-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="40d5c-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="40d5c-112">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="40d5c-113">Stream</span><span class="sxs-lookup"><span data-stu-id="40d5c-113">Stream</span></span>      | <span data-ttu-id="40d5c-114">获取用户执行的 SharePoint 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="40d5c-114">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="40d5c-115">获取文件数</span><span class="sxs-lookup"><span data-stu-id="40d5c-115">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="40d5c-116">Stream</span><span class="sxs-lookup"><span data-stu-id="40d5c-116">Stream</span></span>      | <span data-ttu-id="40d5c-117">获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="40d5c-117">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="40d5c-118">获取用户数</span><span class="sxs-lookup"><span data-stu-id="40d5c-118">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="40d5c-119">Stream</span><span class="sxs-lookup"><span data-stu-id="40d5c-119">Stream</span></span>      | <span data-ttu-id="40d5c-120">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="40d5c-120">Get the trend in the number of active users.</span></span> <span data-ttu-id="40d5c-121">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="40d5c-121">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="40d5c-122">获取页面数</span><span class="sxs-lookup"><span data-stu-id="40d5c-122">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="40d5c-123">Stream</span><span class="sxs-lookup"><span data-stu-id="40d5c-123">Stream</span></span>      | <span data-ttu-id="40d5c-124">获取用户访问的唯一页面数。</span><span class="sxs-lookup"><span data-stu-id="40d5c-124">Get the number of unique pages visited by users.</span></span> |
