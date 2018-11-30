---
title: Office 365 组活动报表
description: 组活动报表可用于深入了解组织中的 Office 365 组活动，并了解正在创建和使用多少个 Office 365 组。
ms.openlocfilehash: eede60c27a9de2eb5d8dcb9636cb6687ffc76c1b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009836"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="a43c4-103">Office 365 组活动报表</span><span class="sxs-lookup"><span data-stu-id="a43c4-103">Office 365 Groups activity reports</span></span>

<span data-ttu-id="a43c4-104">组活动报表可用于深入了解组织中的 Office 365 组活动，并了解正在创建和使用多少个 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="a43c4-104">You can use the Groups activity reports to gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 Groups are being created and used.</span></span>

> <span data-ttu-id="a43c4-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="a43c4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="a43c4-106">报表</span><span class="sxs-lookup"><span data-stu-id="a43c4-106">Reports</span></span>

| <span data-ttu-id="a43c4-107">函数</span><span class="sxs-lookup"><span data-stu-id="a43c4-107">Function</span></span>                                 | <span data-ttu-id="a43c4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a43c4-108">Return Type</span></span> | <span data-ttu-id="a43c4-109">说明</span><span class="sxs-lookup"><span data-stu-id="a43c4-109">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="a43c4-110">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="a43c4-110">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="a43c4-111">Stream</span><span class="sxs-lookup"><span data-stu-id="a43c4-111">Stream</span></span>          | <span data-ttu-id="a43c4-112">获取组执行的 Office 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a43c4-112">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="a43c4-113">获取活动数</span><span class="sxs-lookup"><span data-stu-id="a43c4-113">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="a43c4-114">Stream</span><span class="sxs-lookup"><span data-stu-id="a43c4-114">Stream</span></span>          | <span data-ttu-id="a43c4-115">获取跨组工作负载的组活动数。</span><span class="sxs-lookup"><span data-stu-id="a43c4-115">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="a43c4-116">获取组数</span><span class="sxs-lookup"><span data-stu-id="a43c4-116">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="a43c4-117">Stream</span><span class="sxs-lookup"><span data-stu-id="a43c4-117">Stream</span></span>          | <span data-ttu-id="a43c4-118">获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。</span><span class="sxs-lookup"><span data-stu-id="a43c4-118">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="a43c4-119">获取存储</span><span class="sxs-lookup"><span data-stu-id="a43c4-119">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="a43c4-120">Stream</span><span class="sxs-lookup"><span data-stu-id="a43c4-120">Stream</span></span>          | <span data-ttu-id="a43c4-121">获取跨所有组邮箱和组网站使用的总存储。</span><span class="sxs-lookup"><span data-stu-id="a43c4-121">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="a43c4-122">获取文件数</span><span class="sxs-lookup"><span data-stu-id="a43c4-122">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="a43c4-123">Stream</span><span class="sxs-lookup"><span data-stu-id="a43c4-123">Stream</span></span>          | <span data-ttu-id="a43c4-124">获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="a43c4-124">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
