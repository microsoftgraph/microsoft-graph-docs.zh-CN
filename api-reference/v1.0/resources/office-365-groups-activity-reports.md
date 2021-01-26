---
title: Microsoft 365 组活动报告
description: 可以使用组活动报告深入了解组织中 Microsoft 365 组的活动，并查看正在创建和使用多少个 Microsoft 365 组。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7470eff43c2c77a63206cf24e0484360bf3371b6
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980995"
---
# <a name="microsoft-365-groups-activity-reports"></a><span data-ttu-id="410ca-103">Microsoft 365 组活动报告</span><span class="sxs-lookup"><span data-stu-id="410ca-103">Microsoft 365 groups activity reports</span></span>

<span data-ttu-id="410ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="410ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="410ca-105">可以使用组活动报告深入了解组织中 Microsoft 365 组的活动，并查看正在创建和使用多少个 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="410ca-105">You can use the Groups activity reports to gain insights into the activity of Microsoft 365 groups in your organization and see how many Microsoft 365 groups are being created and used.</span></span>

> <span data-ttu-id="410ca-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - Microsoft 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="410ca-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="410ca-107">报告</span><span class="sxs-lookup"><span data-stu-id="410ca-107">Reports</span></span>

| <span data-ttu-id="410ca-108">函数</span><span class="sxs-lookup"><span data-stu-id="410ca-108">Function</span></span>                                 | <span data-ttu-id="410ca-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="410ca-109">Return Type</span></span> | <span data-ttu-id="410ca-110">说明</span><span class="sxs-lookup"><span data-stu-id="410ca-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="410ca-111">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="410ca-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="410ca-112">Stream</span><span class="sxs-lookup"><span data-stu-id="410ca-112">Stream</span></span>          | <span data-ttu-id="410ca-113">按组获取有关 Microsoft 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="410ca-113">Get details about Microsoft 365 groups activity by group.</span></span> |
| [<span data-ttu-id="410ca-114">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="410ca-114">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="410ca-115">Stream</span><span class="sxs-lookup"><span data-stu-id="410ca-115">Stream</span></span>          | <span data-ttu-id="410ca-116">获取跨组工作负载的组活动数。</span><span class="sxs-lookup"><span data-stu-id="410ca-116">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="410ca-117">获取组数</span><span class="sxs-lookup"><span data-stu-id="410ca-117">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="410ca-118">Stream</span><span class="sxs-lookup"><span data-stu-id="410ca-118">Stream</span></span>          | <span data-ttu-id="410ca-119">获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。</span><span class="sxs-lookup"><span data-stu-id="410ca-119">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="410ca-120">获取存储</span><span class="sxs-lookup"><span data-stu-id="410ca-120">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="410ca-121">Stream</span><span class="sxs-lookup"><span data-stu-id="410ca-121">Stream</span></span>          | <span data-ttu-id="410ca-122">获取跨所有组邮箱和组网站使用的总存储。</span><span class="sxs-lookup"><span data-stu-id="410ca-122">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="410ca-123">获取文件数</span><span class="sxs-lookup"><span data-stu-id="410ca-123">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="410ca-124">Stream</span><span class="sxs-lookup"><span data-stu-id="410ca-124">Stream</span></span>          | <span data-ttu-id="410ca-125">获取与 Microsoft 365 组关联的所有组网站中的文件总数及其活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="410ca-125">Get the total number of files and how many of them were active across all group sites associated with a Microsoft 365 group.</span></span> |

