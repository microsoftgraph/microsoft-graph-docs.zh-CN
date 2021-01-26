---
title: Skype for Business 对等活动报表
description: 可以获取组织中点对点活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 6980e17270db042535b07dd2550114e916827285
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983039"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="45f58-104">Skype for Business 对等活动报表</span><span class="sxs-lookup"><span data-stu-id="45f58-104">Skype for Business peer-to-peer activity reports</span></span>

<span data-ttu-id="45f58-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45f58-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45f58-106">可以获取组织中点对点活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="45f58-106">You can get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="45f58-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="45f58-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="45f58-108">**注意：** 有关不同报告视图和名称的详细信息，请参阅 [Microsoft 365 报告 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="45f58-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="45f58-109">报告</span><span class="sxs-lookup"><span data-stu-id="45f58-109">Reports</span></span>

| <span data-ttu-id="45f58-110">函数</span><span class="sxs-lookup"><span data-stu-id="45f58-110">Function</span></span>                                 | <span data-ttu-id="45f58-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="45f58-111">CSV return type</span></span> | <span data-ttu-id="45f58-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="45f58-112">JSON return type</span></span>                         | <span data-ttu-id="45f58-113">说明</span><span class="sxs-lookup"><span data-stu-id="45f58-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="45f58-114">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="45f58-114">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="45f58-115">Stream</span><span class="sxs-lookup"><span data-stu-id="45f58-115">Stream</span></span>          | [<span data-ttu-id="45f58-116">skypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="45f58-116">skypeForBusinessPeerToPeerActivityCounts</span></span>](../resources/skypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="45f58-117">获取使用情况趋势，即组织中召开的会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="45f58-117">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="45f58-118">会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="45f58-118">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="45f58-119">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="45f58-119">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="45f58-120">Stream</span><span class="sxs-lookup"><span data-stu-id="45f58-120">Stream</span></span>          | [<span data-ttu-id="45f58-121">skypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="45f58-121">skypeForBusinessPeerToPeerActivityUserCounts</span></span>](../resources/skypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="45f58-122">获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="45f58-122">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="45f58-123">对等会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="45f58-123">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="45f58-124">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="45f58-124">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="45f58-125">Stream</span><span class="sxs-lookup"><span data-stu-id="45f58-125">Stream</span></span>          | [<span data-ttu-id="45f58-126">skypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="45f58-126">skypeForBusinessPeerToPeerActivityMinuteCounts</span></span>](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="45f58-127">获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="45f58-127">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="45f58-128">会话类型包括音频和视频。</span><span class="sxs-lookup"><span data-stu-id="45f58-128">Types of sessions include audio and video.</span></span> |


