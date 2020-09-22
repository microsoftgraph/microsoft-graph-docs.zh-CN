---
title: Microsoft 365 组活动报告
description: 您可以深入了解组织中的 Microsoft 365 组活动，并查看创建和使用了多少个 Microsoft 365 组。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: fbe657da65955410a7ea38e3aafdef9d1d853e09
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021236"
---
# <a name="microsoft-365-groups-activity-reports"></a><span data-ttu-id="3ecd4-103">Microsoft 365 组活动报告</span><span class="sxs-lookup"><span data-stu-id="3ecd4-103">Microsoft 365 groups activity reports</span></span>

<span data-ttu-id="3ecd4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ecd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ecd4-105">您可以深入了解组织中的 Microsoft 365 组活动，并查看创建和使用了多少个 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="3ecd4-105">You can gain insights into the activity of Microsoft 365 groups in your organization and see how many Microsoft 365 groups are being created and used.</span></span>

> <span data-ttu-id="3ecd4-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [microsoft 365 报表-microsoft 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="3ecd4-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="3ecd4-107">报表</span><span class="sxs-lookup"><span data-stu-id="3ecd4-107">Reports</span></span>

| <span data-ttu-id="3ecd4-108">函数</span><span class="sxs-lookup"><span data-stu-id="3ecd4-108">Function</span></span>                                 | <span data-ttu-id="3ecd4-109">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="3ecd4-109">CSV return type</span></span> | <span data-ttu-id="3ecd4-110">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="3ecd4-110">JSON return type</span></span>                         | <span data-ttu-id="3ecd4-111">说明</span><span class="sxs-lookup"><span data-stu-id="3ecd4-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="3ecd4-112">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="3ecd4-112">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="3ecd4-113">Stream</span><span class="sxs-lookup"><span data-stu-id="3ecd4-113">Stream</span></span>          | [<span data-ttu-id="3ecd4-114">office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="3ecd4-114">office365GroupsActivityDetail</span></span>](../resources/office365groupsactivitydetail.md) | <span data-ttu-id="3ecd4-115">按组获取有关 Microsoft 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3ecd4-115">Get details about Microsoft 365 groups activity by group.</span></span> |
| [<span data-ttu-id="3ecd4-116">获取活动数</span><span class="sxs-lookup"><span data-stu-id="3ecd4-116">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="3ecd4-117">Stream</span><span class="sxs-lookup"><span data-stu-id="3ecd4-117">Stream</span></span>          | [<span data-ttu-id="3ecd4-118">office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="3ecd4-118">office365GroupsActivityCounts</span></span>](../resources/office365groupsactivitycounts.md) | <span data-ttu-id="3ecd4-119">获取跨组工作负载的组活动数。</span><span class="sxs-lookup"><span data-stu-id="3ecd4-119">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="3ecd4-120">获取组数</span><span class="sxs-lookup"><span data-stu-id="3ecd4-120">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="3ecd4-121">Stream</span><span class="sxs-lookup"><span data-stu-id="3ecd4-121">Stream</span></span>          | [<span data-ttu-id="3ecd4-122">office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="3ecd4-122">office365GroupsActivityGroupCounts</span></span>](../resources/office365groupsactivitygroupcounts.md) | <span data-ttu-id="3ecd4-123">获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。</span><span class="sxs-lookup"><span data-stu-id="3ecd4-123">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="3ecd4-124">获取存储</span><span class="sxs-lookup"><span data-stu-id="3ecd4-124">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="3ecd4-125">Stream</span><span class="sxs-lookup"><span data-stu-id="3ecd4-125">Stream</span></span>          | [<span data-ttu-id="3ecd4-126">office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="3ecd4-126">office365GroupsActivityStorage</span></span>](../resources/office365groupsactivitystorage.md) | <span data-ttu-id="3ecd4-127">获取跨所有组邮箱和组网站使用的总存储。</span><span class="sxs-lookup"><span data-stu-id="3ecd4-127">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="3ecd4-128">获取文件数</span><span class="sxs-lookup"><span data-stu-id="3ecd4-128">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="3ecd4-129">Stream</span><span class="sxs-lookup"><span data-stu-id="3ecd4-129">Stream</span></span>          | [<span data-ttu-id="3ecd4-130">office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="3ecd4-130">office365GroupsActivityFileCounts</span></span>](../resources/office365groupsactivityfilecounts.md) | <span data-ttu-id="3ecd4-131">获取总文件数以及与 Microsoft 365 组关联的所有组网站中有多少个处于活动状态的文件。</span><span class="sxs-lookup"><span data-stu-id="3ecd4-131">Get the total number of files and how many of them were active across all group sites associated with a Microsoft 365 group.</span></span> |


