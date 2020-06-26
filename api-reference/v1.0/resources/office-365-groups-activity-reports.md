---
title: Microsoft 365 组活动报告
description: 您可以使用组活动报告来深入了解组织中的 Microsoft 365 组活动，并查看创建和使用了多少个 Microsoft 365 组。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0cd0dfc07813714d376a38125835917c712e7ebe
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898154"
---
# <a name="microsoft-365-groups-activity-reports"></a><span data-ttu-id="16aff-103">Microsoft 365 组活动报告</span><span class="sxs-lookup"><span data-stu-id="16aff-103">Microsoft 365 groups activity reports</span></span>

<span data-ttu-id="16aff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16aff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16aff-105">您可以使用组活动报告来深入了解组织中的 Microsoft 365 组活动，并查看创建和使用了多少个 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="16aff-105">You can use the Groups activity reports to gain insights into the activity of Microsoft 365 groups in your organization and see how many Microsoft 365 groups are being created and used.</span></span>

> <span data-ttu-id="16aff-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅[microsoft 365 报表-microsoft 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="16aff-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="16aff-107">报表</span><span class="sxs-lookup"><span data-stu-id="16aff-107">Reports</span></span>

| <span data-ttu-id="16aff-108">函数</span><span class="sxs-lookup"><span data-stu-id="16aff-108">Function</span></span>                                 | <span data-ttu-id="16aff-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="16aff-109">Return Type</span></span> | <span data-ttu-id="16aff-110">说明</span><span class="sxs-lookup"><span data-stu-id="16aff-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="16aff-111">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="16aff-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="16aff-112">Stream</span><span class="sxs-lookup"><span data-stu-id="16aff-112">Stream</span></span>          | <span data-ttu-id="16aff-113">按组获取有关 Microsoft 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="16aff-113">Get details about Microsoft 365 groups activity by group.</span></span> |
| [<span data-ttu-id="16aff-114">获取活动数</span><span class="sxs-lookup"><span data-stu-id="16aff-114">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="16aff-115">Stream</span><span class="sxs-lookup"><span data-stu-id="16aff-115">Stream</span></span>          | <span data-ttu-id="16aff-116">获取跨组工作负载的组活动数。</span><span class="sxs-lookup"><span data-stu-id="16aff-116">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="16aff-117">获取组数</span><span class="sxs-lookup"><span data-stu-id="16aff-117">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="16aff-118">Stream</span><span class="sxs-lookup"><span data-stu-id="16aff-118">Stream</span></span>          | <span data-ttu-id="16aff-119">获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。</span><span class="sxs-lookup"><span data-stu-id="16aff-119">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="16aff-120">获取存储</span><span class="sxs-lookup"><span data-stu-id="16aff-120">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="16aff-121">Stream</span><span class="sxs-lookup"><span data-stu-id="16aff-121">Stream</span></span>          | <span data-ttu-id="16aff-122">获取跨所有组邮箱和组网站使用的总存储。</span><span class="sxs-lookup"><span data-stu-id="16aff-122">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="16aff-123">获取文件数</span><span class="sxs-lookup"><span data-stu-id="16aff-123">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="16aff-124">Stream</span><span class="sxs-lookup"><span data-stu-id="16aff-124">Stream</span></span>          | <span data-ttu-id="16aff-125">获取总文件数以及与 Microsoft 365 组关联的所有组网站中有多少个处于活动状态的文件。</span><span class="sxs-lookup"><span data-stu-id="16aff-125">Get the total number of files and how many of them were active across all group sites associated with a Microsoft 365 group.</span></span> |
