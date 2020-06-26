---
title: Yammer 组活动报表
description: 您可以深入了解组织中的 Yammer 组活动，并查看正在创建和使用的 Yammer 组的数量。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: cdeb94c9b5b687ab9584a236daaafb7c018a809c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897468"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="f3080-103">Yammer 组活动报表</span><span class="sxs-lookup"><span data-stu-id="f3080-103">Yammer groups activity reports</span></span>

<span data-ttu-id="f3080-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3080-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3080-105">您可以深入了解组织中的 Yammer 组活动，并查看正在创建和使用的 Yammer 组的数量。</span><span class="sxs-lookup"><span data-stu-id="f3080-105">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="f3080-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="f3080-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="f3080-107">报表</span><span class="sxs-lookup"><span data-stu-id="f3080-107">Reports</span></span>

| <span data-ttu-id="f3080-108">函数</span><span class="sxs-lookup"><span data-stu-id="f3080-108">Function</span></span>                                 | <span data-ttu-id="f3080-109">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="f3080-109">CSV return type</span></span> | <span data-ttu-id="f3080-110">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="f3080-110">JSON return type</span></span>                         | <span data-ttu-id="f3080-111">说明</span><span class="sxs-lookup"><span data-stu-id="f3080-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="f3080-112">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="f3080-112">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="f3080-113">Stream</span><span class="sxs-lookup"><span data-stu-id="f3080-113">Stream</span></span>          | [<span data-ttu-id="f3080-114">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="f3080-114">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="f3080-115">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f3080-115">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="f3080-116">获取组数</span><span class="sxs-lookup"><span data-stu-id="f3080-116">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="f3080-117">Stream</span><span class="sxs-lookup"><span data-stu-id="f3080-117">Stream</span></span>          | [<span data-ttu-id="f3080-118">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="f3080-118">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="f3080-119">获取存在的总组数，以及有多少组包含组对话活动。</span><span class="sxs-lookup"><span data-stu-id="f3080-119">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="f3080-120">获取活动数</span><span class="sxs-lookup"><span data-stu-id="f3080-120">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="f3080-121">Stream</span><span class="sxs-lookup"><span data-stu-id="f3080-121">Stream</span></span>          | [<span data-ttu-id="f3080-122">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="f3080-122">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="f3080-123">获取组中已发布、已阅读和已赞的 Yammer 消息数。</span><span class="sxs-lookup"><span data-stu-id="f3080-123">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
