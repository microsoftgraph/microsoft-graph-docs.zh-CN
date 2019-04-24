---
title: Office 365 组活动报表
description: 组活动报表可用于深入了解组织中的 Office 365 组活动，并了解正在创建和使用多少个 Office 365 组。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5d8c414034a110db64b770a72fe2e3540806acdd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462947"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="e8783-103">Office 365 组活动报表</span><span class="sxs-lookup"><span data-stu-id="e8783-103">Office 365 Groups activity reports</span></span>

<span data-ttu-id="e8783-104">组活动报表可用于深入了解组织中的 Office 365 组活动，并了解正在创建和使用多少个 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="e8783-104">You can use the Groups activity reports to gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 Groups are being created and used.</span></span>

> <span data-ttu-id="e8783-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="e8783-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="e8783-106">报表</span><span class="sxs-lookup"><span data-stu-id="e8783-106">Reports</span></span>

| <span data-ttu-id="e8783-107">函数</span><span class="sxs-lookup"><span data-stu-id="e8783-107">Function</span></span>                                 | <span data-ttu-id="e8783-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e8783-108">Return Type</span></span> | <span data-ttu-id="e8783-109">说明</span><span class="sxs-lookup"><span data-stu-id="e8783-109">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="e8783-110">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="e8783-110">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="e8783-111">Stream</span><span class="sxs-lookup"><span data-stu-id="e8783-111">Stream</span></span>          | <span data-ttu-id="e8783-112">获取组执行的 Office 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e8783-112">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="e8783-113">获取活动数</span><span class="sxs-lookup"><span data-stu-id="e8783-113">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="e8783-114">Stream</span><span class="sxs-lookup"><span data-stu-id="e8783-114">Stream</span></span>          | <span data-ttu-id="e8783-115">获取跨组工作负载的组活动数。</span><span class="sxs-lookup"><span data-stu-id="e8783-115">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="e8783-116">获取组数</span><span class="sxs-lookup"><span data-stu-id="e8783-116">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="e8783-117">Stream</span><span class="sxs-lookup"><span data-stu-id="e8783-117">Stream</span></span>          | <span data-ttu-id="e8783-118">获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。</span><span class="sxs-lookup"><span data-stu-id="e8783-118">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="e8783-119">获取存储</span><span class="sxs-lookup"><span data-stu-id="e8783-119">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="e8783-120">Stream</span><span class="sxs-lookup"><span data-stu-id="e8783-120">Stream</span></span>          | <span data-ttu-id="e8783-121">获取跨所有组邮箱和组网站使用的总存储。</span><span class="sxs-lookup"><span data-stu-id="e8783-121">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="e8783-122">获取文件数</span><span class="sxs-lookup"><span data-stu-id="e8783-122">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="e8783-123">Stream</span><span class="sxs-lookup"><span data-stu-id="e8783-123">Stream</span></span>          | <span data-ttu-id="e8783-124">获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="e8783-124">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
