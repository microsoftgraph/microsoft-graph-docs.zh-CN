---
title: Yammer 组活动报表
description: 可以在组织中获得的 Yammer 组活动见解并查看多少个 Yammer 组被创建和使用。
localization_priority: Normal
ms.openlocfilehash: 90be4037871480b7d694f4f9089d5f62064c9d2b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890669"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="4dcba-103">Yammer 组活动报表</span><span class="sxs-lookup"><span data-stu-id="4dcba-103">Yammer groups activity reports</span></span>

> <span data-ttu-id="4dcba-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4dcba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dcba-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4dcba-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="4dcba-106">在 Microsoft Graph 中国由 21Vianet 不支持这些 Api。</span><span class="sxs-lookup"><span data-stu-id="4dcba-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="4dcba-107">可以在组织中获得的 Yammer 组活动见解并查看多少个 Yammer 组被创建和使用。</span><span class="sxs-lookup"><span data-stu-id="4dcba-107">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="4dcba-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="4dcba-108">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="4dcba-109">报表</span><span class="sxs-lookup"><span data-stu-id="4dcba-109">Reports</span></span>

| <span data-ttu-id="4dcba-110">函数</span><span class="sxs-lookup"><span data-stu-id="4dcba-110">Function</span></span>                                 | <span data-ttu-id="4dcba-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="4dcba-111">CSV return type</span></span> | <span data-ttu-id="4dcba-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="4dcba-112">JSON return type</span></span>                         | <span data-ttu-id="4dcba-113">说明</span><span class="sxs-lookup"><span data-stu-id="4dcba-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="4dcba-114">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="4dcba-114">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="4dcba-115">Stream</span><span class="sxs-lookup"><span data-stu-id="4dcba-115">Stream</span></span>          | [<span data-ttu-id="4dcba-116">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="4dcba-116">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="4dcba-117">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4dcba-117">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="4dcba-118">获取组数</span><span class="sxs-lookup"><span data-stu-id="4dcba-118">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="4dcba-119">Stream</span><span class="sxs-lookup"><span data-stu-id="4dcba-119">Stream</span></span>          | [<span data-ttu-id="4dcba-120">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="4dcba-120">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="4dcba-121">获取存在的总组数，以及有多少组包含组对话活动。</span><span class="sxs-lookup"><span data-stu-id="4dcba-121">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="4dcba-122">获取活动数</span><span class="sxs-lookup"><span data-stu-id="4dcba-122">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="4dcba-123">Stream</span><span class="sxs-lookup"><span data-stu-id="4dcba-123">Stream</span></span>          | [<span data-ttu-id="4dcba-124">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4dcba-124">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="4dcba-125">获取组中已发布、已阅读和已赞的 Yammer 消息数。</span><span class="sxs-lookup"><span data-stu-id="4dcba-125">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
