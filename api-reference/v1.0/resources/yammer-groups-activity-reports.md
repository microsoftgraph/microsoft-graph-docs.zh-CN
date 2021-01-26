---
title: Yammer 组活动报表
description: Yammer 组活动报表可用于深入了解组织中的 Yammer 组活动，并了解正在创建和使用多少个 Yammer 组。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: cb821497980e4d048249c7da37100c78d45f6472
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980617"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="76282-103">Yammer 组活动报表</span><span class="sxs-lookup"><span data-stu-id="76282-103">Yammer groups activity reports</span></span>

<span data-ttu-id="76282-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76282-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76282-105">Yammer 组活动报表可用于深入了解组织中的 Yammer 组活动，并了解正在创建和使用多少个 Yammer 组。</span><span class="sxs-lookup"><span data-stu-id="76282-105">You can use the Yammer groups activity reports to gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="76282-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="76282-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="76282-107">报告</span><span class="sxs-lookup"><span data-stu-id="76282-107">Reports</span></span>

| <span data-ttu-id="76282-108">函数</span><span class="sxs-lookup"><span data-stu-id="76282-108">Function</span></span>                                 | <span data-ttu-id="76282-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="76282-109">Return Type</span></span> | <span data-ttu-id="76282-110">说明</span><span class="sxs-lookup"><span data-stu-id="76282-110">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="76282-111">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="76282-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="76282-112">Stream</span><span class="sxs-lookup"><span data-stu-id="76282-112">Stream</span></span>      | <span data-ttu-id="76282-113">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="76282-113">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="76282-114">获取组数</span><span class="sxs-lookup"><span data-stu-id="76282-114">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="76282-115">Stream</span><span class="sxs-lookup"><span data-stu-id="76282-115">Stream</span></span>      | <span data-ttu-id="76282-116">获取存在的总组数，以及有多少组包含组对话活动。</span><span class="sxs-lookup"><span data-stu-id="76282-116">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="76282-117">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="76282-117">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="76282-118">Stream</span><span class="sxs-lookup"><span data-stu-id="76282-118">Stream</span></span>      | <span data-ttu-id="76282-119">获取组中已发布、已阅读和已赞的 Yammer 消息数。</span><span class="sxs-lookup"><span data-stu-id="76282-119">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |

