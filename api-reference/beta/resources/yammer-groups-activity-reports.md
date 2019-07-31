---
title: Yammer 组活动报表
description: 您可以深入了解组织中的 Yammer 组活动, 并查看正在创建和使用的 Yammer 组的数量。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 07a78a4b2047e03beee611443240f56739f76b4f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963836"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="17594-103">Yammer 组活动报表</span><span class="sxs-lookup"><span data-stu-id="17594-103">Yammer groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17594-104">您可以深入了解组织中的 Yammer 组活动, 并查看正在创建和使用的 Yammer 组的数量。</span><span class="sxs-lookup"><span data-stu-id="17594-104">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="17594-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="17594-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="17594-106">报表</span><span class="sxs-lookup"><span data-stu-id="17594-106">Reports</span></span>

| <span data-ttu-id="17594-107">函数</span><span class="sxs-lookup"><span data-stu-id="17594-107">Function</span></span>                                 | <span data-ttu-id="17594-108">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="17594-108">CSV return type</span></span> | <span data-ttu-id="17594-109">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="17594-109">JSON return type</span></span>                         | <span data-ttu-id="17594-110">说明</span><span class="sxs-lookup"><span data-stu-id="17594-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="17594-111">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="17594-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="17594-112">流</span><span class="sxs-lookup"><span data-stu-id="17594-112">Stream</span></span>          | [<span data-ttu-id="17594-113">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="17594-113">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="17594-114">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="17594-114">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="17594-115">获取组数</span><span class="sxs-lookup"><span data-stu-id="17594-115">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="17594-116">Stream</span><span class="sxs-lookup"><span data-stu-id="17594-116">Stream</span></span>          | [<span data-ttu-id="17594-117">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="17594-117">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="17594-118">获取存在的总组数，以及有多少组包含组对话活动。</span><span class="sxs-lookup"><span data-stu-id="17594-118">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="17594-119">获取活动数</span><span class="sxs-lookup"><span data-stu-id="17594-119">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="17594-120">Stream</span><span class="sxs-lookup"><span data-stu-id="17594-120">Stream</span></span>          | [<span data-ttu-id="17594-121">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="17594-121">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="17594-122">获取组中已发布、已阅读和已赞的 Yammer 消息数。</span><span class="sxs-lookup"><span data-stu-id="17594-122">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
