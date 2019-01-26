---
title: Office 365 组活动报表
description: 可以在组织中获得的 Office 365 组活动见解并查看多少个 Office 365 组被创建和使用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e698a1096d244b864bbb15cf06c16e8cf79ff1f2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572197"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="ab019-103">Office 365 组活动报表</span><span class="sxs-lookup"><span data-stu-id="ab019-103">Office 365 Groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab019-104">可以在组织中获得的 Office 365 组活动见解并查看多少个 Office 365 组被创建和使用。</span><span class="sxs-lookup"><span data-stu-id="ab019-104">You can gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 groups are being created and used.</span></span>

> <span data-ttu-id="ab019-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="ab019-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="ab019-106">报表</span><span class="sxs-lookup"><span data-stu-id="ab019-106">Reports</span></span>

| <span data-ttu-id="ab019-107">函数</span><span class="sxs-lookup"><span data-stu-id="ab019-107">Function</span></span>                                 | <span data-ttu-id="ab019-108">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="ab019-108">CSV return type</span></span> | <span data-ttu-id="ab019-109">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="ab019-109">JSON return type</span></span>                         | <span data-ttu-id="ab019-110">说明</span><span class="sxs-lookup"><span data-stu-id="ab019-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ab019-111">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="ab019-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="ab019-112">Stream</span><span class="sxs-lookup"><span data-stu-id="ab019-112">Stream</span></span>          | [<span data-ttu-id="ab019-113">office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="ab019-113">office365GroupsActivityDetail</span></span>](../resources/office365groupsactivitydetail.md) | <span data-ttu-id="ab019-114">获取组执行的 Office 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ab019-114">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="ab019-115">获取活动数</span><span class="sxs-lookup"><span data-stu-id="ab019-115">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="ab019-116">Stream</span><span class="sxs-lookup"><span data-stu-id="ab019-116">Stream</span></span>          | [<span data-ttu-id="ab019-117">office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ab019-117">office365GroupsActivityCounts</span></span>](../resources/office365groupsactivitycounts.md) | <span data-ttu-id="ab019-118">获取跨组工作负载的组活动数。</span><span class="sxs-lookup"><span data-stu-id="ab019-118">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="ab019-119">获取组数</span><span class="sxs-lookup"><span data-stu-id="ab019-119">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="ab019-120">Stream</span><span class="sxs-lookup"><span data-stu-id="ab019-120">Stream</span></span>          | [<span data-ttu-id="ab019-121">office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="ab019-121">office365GroupsActivityGroupCounts</span></span>](../resources/office365groupsactivitygroupcounts.md) | <span data-ttu-id="ab019-122">获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。</span><span class="sxs-lookup"><span data-stu-id="ab019-122">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="ab019-123">获取存储</span><span class="sxs-lookup"><span data-stu-id="ab019-123">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="ab019-124">Stream</span><span class="sxs-lookup"><span data-stu-id="ab019-124">Stream</span></span>          | [<span data-ttu-id="ab019-125">office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="ab019-125">office365GroupsActivityStorage</span></span>](../resources/office365groupsactivitystorage.md) | <span data-ttu-id="ab019-126">获取跨所有组邮箱和组网站使用的总存储。</span><span class="sxs-lookup"><span data-stu-id="ab019-126">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="ab019-127">获取文件数</span><span class="sxs-lookup"><span data-stu-id="ab019-127">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="ab019-128">Stream</span><span class="sxs-lookup"><span data-stu-id="ab019-128">Stream</span></span>          | [<span data-ttu-id="ab019-129">office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="ab019-129">office365GroupsActivityFileCounts</span></span>](../resources/office365groupsactivityfilecounts.md) | <span data-ttu-id="ab019-130">获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="ab019-130">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
