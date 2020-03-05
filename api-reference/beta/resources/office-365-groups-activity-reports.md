---
title: Office 365 组活动报表
description: 您可以深入了解组织中的 Office 365 组的活动，并查看创建和使用了多少个 Office 365 组。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 1a78de815ff75b5e7e65626235799d4a2249ee84
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522496"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="90aaa-103">Office 365 组活动报表</span><span class="sxs-lookup"><span data-stu-id="90aaa-103">Office 365 Groups activity reports</span></span>

<span data-ttu-id="90aaa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="90aaa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90aaa-105">您可以深入了解组织中的 Office 365 组的活动，并查看创建和使用了多少个 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="90aaa-105">You can gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 groups are being created and used.</span></span>

> <span data-ttu-id="90aaa-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="90aaa-106">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="90aaa-107">报表</span><span class="sxs-lookup"><span data-stu-id="90aaa-107">Reports</span></span>

| <span data-ttu-id="90aaa-108">函数</span><span class="sxs-lookup"><span data-stu-id="90aaa-108">Function</span></span>                                 | <span data-ttu-id="90aaa-109">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="90aaa-109">CSV return type</span></span> | <span data-ttu-id="90aaa-110">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="90aaa-110">JSON return type</span></span>                         | <span data-ttu-id="90aaa-111">说明</span><span class="sxs-lookup"><span data-stu-id="90aaa-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="90aaa-112">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="90aaa-112">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="90aaa-113">Stream</span><span class="sxs-lookup"><span data-stu-id="90aaa-113">Stream</span></span>          | [<span data-ttu-id="90aaa-114">office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="90aaa-114">office365GroupsActivityDetail</span></span>](../resources/office365groupsactivitydetail.md) | <span data-ttu-id="90aaa-115">获取组执行的 Office 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="90aaa-115">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="90aaa-116">获取活动数</span><span class="sxs-lookup"><span data-stu-id="90aaa-116">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="90aaa-117">Stream</span><span class="sxs-lookup"><span data-stu-id="90aaa-117">Stream</span></span>          | [<span data-ttu-id="90aaa-118">office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="90aaa-118">office365GroupsActivityCounts</span></span>](../resources/office365groupsactivitycounts.md) | <span data-ttu-id="90aaa-119">获取跨组工作负载的组活动数。</span><span class="sxs-lookup"><span data-stu-id="90aaa-119">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="90aaa-120">获取组数</span><span class="sxs-lookup"><span data-stu-id="90aaa-120">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="90aaa-121">Stream</span><span class="sxs-lookup"><span data-stu-id="90aaa-121">Stream</span></span>          | [<span data-ttu-id="90aaa-122">office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="90aaa-122">office365GroupsActivityGroupCounts</span></span>](../resources/office365groupsactivitygroupcounts.md) | <span data-ttu-id="90aaa-123">获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。</span><span class="sxs-lookup"><span data-stu-id="90aaa-123">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="90aaa-124">获取存储</span><span class="sxs-lookup"><span data-stu-id="90aaa-124">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="90aaa-125">Stream</span><span class="sxs-lookup"><span data-stu-id="90aaa-125">Stream</span></span>          | [<span data-ttu-id="90aaa-126">office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="90aaa-126">office365GroupsActivityStorage</span></span>](../resources/office365groupsactivitystorage.md) | <span data-ttu-id="90aaa-127">获取跨所有组邮箱和组网站使用的总存储。</span><span class="sxs-lookup"><span data-stu-id="90aaa-127">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="90aaa-128">获取文件数</span><span class="sxs-lookup"><span data-stu-id="90aaa-128">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="90aaa-129">Stream</span><span class="sxs-lookup"><span data-stu-id="90aaa-129">Stream</span></span>          | [<span data-ttu-id="90aaa-130">office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="90aaa-130">office365GroupsActivityFileCounts</span></span>](../resources/office365groupsactivityfilecounts.md) | <span data-ttu-id="90aaa-131">获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="90aaa-131">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
