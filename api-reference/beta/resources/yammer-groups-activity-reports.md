---
title: Yammer 组活动报表
description: 您可以深入了解组织中的 Yammer 组活动，并查看正在创建和使用的 Yammer 组的数量。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 8a2ebade9af9133febab39b9a9ec95a3536d246b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519041"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="342bf-103">Yammer 组活动报表</span><span class="sxs-lookup"><span data-stu-id="342bf-103">Yammer groups activity reports</span></span>

<span data-ttu-id="342bf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="342bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="342bf-105">您可以深入了解组织中的 Yammer 组活动，并查看正在创建和使用的 Yammer 组的数量。</span><span class="sxs-lookup"><span data-stu-id="342bf-105">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="342bf-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="342bf-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="342bf-107">报表</span><span class="sxs-lookup"><span data-stu-id="342bf-107">Reports</span></span>

| <span data-ttu-id="342bf-108">函数</span><span class="sxs-lookup"><span data-stu-id="342bf-108">Function</span></span>                                 | <span data-ttu-id="342bf-109">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="342bf-109">CSV return type</span></span> | <span data-ttu-id="342bf-110">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="342bf-110">JSON return type</span></span>                         | <span data-ttu-id="342bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="342bf-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="342bf-112">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="342bf-112">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="342bf-113">Stream</span><span class="sxs-lookup"><span data-stu-id="342bf-113">Stream</span></span>          | [<span data-ttu-id="342bf-114">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="342bf-114">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="342bf-115">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="342bf-115">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="342bf-116">获取组数</span><span class="sxs-lookup"><span data-stu-id="342bf-116">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="342bf-117">Stream</span><span class="sxs-lookup"><span data-stu-id="342bf-117">Stream</span></span>          | [<span data-ttu-id="342bf-118">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="342bf-118">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="342bf-119">获取存在的总组数，以及有多少组包含组对话活动。</span><span class="sxs-lookup"><span data-stu-id="342bf-119">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="342bf-120">获取活动数</span><span class="sxs-lookup"><span data-stu-id="342bf-120">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="342bf-121">Stream</span><span class="sxs-lookup"><span data-stu-id="342bf-121">Stream</span></span>          | [<span data-ttu-id="342bf-122">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="342bf-122">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="342bf-123">获取组中已发布、已阅读和已赞的 Yammer 消息数。</span><span class="sxs-lookup"><span data-stu-id="342bf-123">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
