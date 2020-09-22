---
title: Yammer 组活动报表
description: 您可以深入了解组织中的 Yammer 组活动，并查看正在创建和使用的 Yammer 组的数量。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 730836b397fd11799849dcae27ae83f9db815e28
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023735"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="819b6-103">Yammer 组活动报表</span><span class="sxs-lookup"><span data-stu-id="819b6-103">Yammer groups activity reports</span></span>

<span data-ttu-id="819b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="819b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="819b6-105">您可以深入了解组织中的 Yammer 组活动，并查看正在创建和使用的 Yammer 组的数量。</span><span class="sxs-lookup"><span data-stu-id="819b6-105">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="819b6-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表-Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="819b6-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="819b6-107">报表</span><span class="sxs-lookup"><span data-stu-id="819b6-107">Reports</span></span>

| <span data-ttu-id="819b6-108">函数</span><span class="sxs-lookup"><span data-stu-id="819b6-108">Function</span></span>                                 | <span data-ttu-id="819b6-109">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="819b6-109">CSV return type</span></span> | <span data-ttu-id="819b6-110">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="819b6-110">JSON return type</span></span>                         | <span data-ttu-id="819b6-111">说明</span><span class="sxs-lookup"><span data-stu-id="819b6-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="819b6-112">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="819b6-112">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="819b6-113">Stream</span><span class="sxs-lookup"><span data-stu-id="819b6-113">Stream</span></span>          | [<span data-ttu-id="819b6-114">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="819b6-114">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="819b6-115">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="819b6-115">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="819b6-116">获取组数</span><span class="sxs-lookup"><span data-stu-id="819b6-116">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="819b6-117">Stream</span><span class="sxs-lookup"><span data-stu-id="819b6-117">Stream</span></span>          | [<span data-ttu-id="819b6-118">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="819b6-118">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="819b6-119">获取存在的总组数，以及有多少组包含组对话活动。</span><span class="sxs-lookup"><span data-stu-id="819b6-119">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="819b6-120">获取活动数</span><span class="sxs-lookup"><span data-stu-id="819b6-120">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="819b6-121">Stream</span><span class="sxs-lookup"><span data-stu-id="819b6-121">Stream</span></span>          | [<span data-ttu-id="819b6-122">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="819b6-122">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="819b6-123">获取组中已发布、已阅读和已赞的 Yammer 消息数。</span><span class="sxs-lookup"><span data-stu-id="819b6-123">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |


