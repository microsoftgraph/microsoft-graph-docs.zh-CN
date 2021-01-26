---
title: Yammer 组活动报表
description: 您可以深入了解组织中 Yammer 组的活动，并查看创建和使用的 Yammer 组数。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 09c8aa8476886f8bbf7266817449195b4c07aa05
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982423"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="aa92e-103">Yammer 组活动报表</span><span class="sxs-lookup"><span data-stu-id="aa92e-103">Yammer groups activity reports</span></span>

<span data-ttu-id="aa92e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa92e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa92e-105">您可以深入了解组织中 Yammer 组的活动，并查看创建和使用的 Yammer 组数。</span><span class="sxs-lookup"><span data-stu-id="aa92e-105">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="aa92e-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="aa92e-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="aa92e-107">报告</span><span class="sxs-lookup"><span data-stu-id="aa92e-107">Reports</span></span>

| <span data-ttu-id="aa92e-108">函数</span><span class="sxs-lookup"><span data-stu-id="aa92e-108">Function</span></span>                                 | <span data-ttu-id="aa92e-109">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="aa92e-109">CSV return type</span></span> | <span data-ttu-id="aa92e-110">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="aa92e-110">JSON return type</span></span>                         | <span data-ttu-id="aa92e-111">说明</span><span class="sxs-lookup"><span data-stu-id="aa92e-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="aa92e-112">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="aa92e-112">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="aa92e-113">Stream</span><span class="sxs-lookup"><span data-stu-id="aa92e-113">Stream</span></span>          | [<span data-ttu-id="aa92e-114">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="aa92e-114">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="aa92e-115">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="aa92e-115">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="aa92e-116">获取组数</span><span class="sxs-lookup"><span data-stu-id="aa92e-116">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="aa92e-117">Stream</span><span class="sxs-lookup"><span data-stu-id="aa92e-117">Stream</span></span>          | [<span data-ttu-id="aa92e-118">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="aa92e-118">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="aa92e-119">获取存在的总组数，以及有多少组包含组对话活动。</span><span class="sxs-lookup"><span data-stu-id="aa92e-119">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="aa92e-120">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="aa92e-120">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="aa92e-121">Stream</span><span class="sxs-lookup"><span data-stu-id="aa92e-121">Stream</span></span>          | [<span data-ttu-id="aa92e-122">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="aa92e-122">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="aa92e-123">获取组中已发布、已阅读和已赞的 Yammer 消息数。</span><span class="sxs-lookup"><span data-stu-id="aa92e-123">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |


