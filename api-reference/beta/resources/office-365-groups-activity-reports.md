---
title: Microsoft 365 组活动报告
description: 你可以深入了解组织中 Microsoft 365 组的活动，并查看创建和使用的 Microsoft 365 组数。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 0b2f38512ed41fea65f363c8e7ddbef156794fc3
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980764"
---
# <a name="microsoft-365-groups-activity-reports"></a><span data-ttu-id="d3f42-103">Microsoft 365 组活动报告</span><span class="sxs-lookup"><span data-stu-id="d3f42-103">Microsoft 365 groups activity reports</span></span>

<span data-ttu-id="d3f42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3f42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3f42-105">你可以深入了解组织中 Microsoft 365 组的活动，并查看创建和使用的 Microsoft 365 组数。</span><span class="sxs-lookup"><span data-stu-id="d3f42-105">You can gain insights into the activity of Microsoft 365 groups in your organization and see how many Microsoft 365 groups are being created and used.</span></span>

> <span data-ttu-id="d3f42-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - Microsoft 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="d3f42-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="d3f42-107">报告</span><span class="sxs-lookup"><span data-stu-id="d3f42-107">Reports</span></span>

| <span data-ttu-id="d3f42-108">函数</span><span class="sxs-lookup"><span data-stu-id="d3f42-108">Function</span></span>                                 | <span data-ttu-id="d3f42-109">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="d3f42-109">CSV return type</span></span> | <span data-ttu-id="d3f42-110">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="d3f42-110">JSON return type</span></span>                         | <span data-ttu-id="d3f42-111">说明</span><span class="sxs-lookup"><span data-stu-id="d3f42-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="d3f42-112">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="d3f42-112">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="d3f42-113">Stream</span><span class="sxs-lookup"><span data-stu-id="d3f42-113">Stream</span></span>          | [<span data-ttu-id="d3f42-114">office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="d3f42-114">office365GroupsActivityDetail</span></span>](../resources/office365groupsactivitydetail.md) | <span data-ttu-id="d3f42-115">按组获取有关 Microsoft 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d3f42-115">Get details about Microsoft 365 groups activity by group.</span></span> |
| [<span data-ttu-id="d3f42-116">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="d3f42-116">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="d3f42-117">Stream</span><span class="sxs-lookup"><span data-stu-id="d3f42-117">Stream</span></span>          | [<span data-ttu-id="d3f42-118">office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="d3f42-118">office365GroupsActivityCounts</span></span>](../resources/office365groupsactivitycounts.md) | <span data-ttu-id="d3f42-119">获取跨组工作负载的组活动数。</span><span class="sxs-lookup"><span data-stu-id="d3f42-119">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="d3f42-120">获取组数</span><span class="sxs-lookup"><span data-stu-id="d3f42-120">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="d3f42-121">Stream</span><span class="sxs-lookup"><span data-stu-id="d3f42-121">Stream</span></span>          | [<span data-ttu-id="d3f42-122">office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="d3f42-122">office365GroupsActivityGroupCounts</span></span>](../resources/office365groupsactivitygroupcounts.md) | <span data-ttu-id="d3f42-123">获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。</span><span class="sxs-lookup"><span data-stu-id="d3f42-123">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="d3f42-124">获取存储</span><span class="sxs-lookup"><span data-stu-id="d3f42-124">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="d3f42-125">Stream</span><span class="sxs-lookup"><span data-stu-id="d3f42-125">Stream</span></span>          | [<span data-ttu-id="d3f42-126">office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="d3f42-126">office365GroupsActivityStorage</span></span>](../resources/office365groupsactivitystorage.md) | <span data-ttu-id="d3f42-127">获取跨所有组邮箱和组网站使用的总存储。</span><span class="sxs-lookup"><span data-stu-id="d3f42-127">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="d3f42-128">获取文件数</span><span class="sxs-lookup"><span data-stu-id="d3f42-128">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="d3f42-129">Stream</span><span class="sxs-lookup"><span data-stu-id="d3f42-129">Stream</span></span>          | [<span data-ttu-id="d3f42-130">office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="d3f42-130">office365GroupsActivityFileCounts</span></span>](../resources/office365groupsactivityfilecounts.md) | <span data-ttu-id="d3f42-131">获取与 Microsoft 365 组关联的所有组网站中的文件总数及其活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="d3f42-131">Get the total number of files and how many of them were active across all group sites associated with a Microsoft 365 group.</span></span> |


