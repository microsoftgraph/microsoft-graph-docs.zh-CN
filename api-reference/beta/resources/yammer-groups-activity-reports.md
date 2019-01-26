---
title: Yammer 组活动报表
description: 可以在组织中获得的 Yammer 组活动见解并查看多少个 Yammer 组被创建和使用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 07ec3db93088dd00af1b8595e5d059fc2cede774
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576022"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="f3079-103">Yammer 组活动报表</span><span class="sxs-lookup"><span data-stu-id="f3079-103">Yammer groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3079-104">可以在组织中获得的 Yammer 组活动见解并查看多少个 Yammer 组被创建和使用。</span><span class="sxs-lookup"><span data-stu-id="f3079-104">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="f3079-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="f3079-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="f3079-106">报表</span><span class="sxs-lookup"><span data-stu-id="f3079-106">Reports</span></span>

| <span data-ttu-id="f3079-107">函数</span><span class="sxs-lookup"><span data-stu-id="f3079-107">Function</span></span>                                 | <span data-ttu-id="f3079-108">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="f3079-108">CSV return type</span></span> | <span data-ttu-id="f3079-109">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="f3079-109">JSON return type</span></span>                         | <span data-ttu-id="f3079-110">说明</span><span class="sxs-lookup"><span data-stu-id="f3079-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="f3079-111">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="f3079-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="f3079-112">Stream</span><span class="sxs-lookup"><span data-stu-id="f3079-112">Stream</span></span>          | [<span data-ttu-id="f3079-113">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="f3079-113">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="f3079-114">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f3079-114">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="f3079-115">获取组数</span><span class="sxs-lookup"><span data-stu-id="f3079-115">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="f3079-116">Stream</span><span class="sxs-lookup"><span data-stu-id="f3079-116">Stream</span></span>          | [<span data-ttu-id="f3079-117">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="f3079-117">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="f3079-118">获取存在的总组数，以及有多少组包含组对话活动。</span><span class="sxs-lookup"><span data-stu-id="f3079-118">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="f3079-119">获取活动数</span><span class="sxs-lookup"><span data-stu-id="f3079-119">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="f3079-120">Stream</span><span class="sxs-lookup"><span data-stu-id="f3079-120">Stream</span></span>          | [<span data-ttu-id="f3079-121">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="f3079-121">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="f3079-122">获取组中已发布、已阅读和已赞的 Yammer 消息数。</span><span class="sxs-lookup"><span data-stu-id="f3079-122">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
