---
title: Skype for Business 对等活动报表
description: Skype for Business 对等活动报表可用于获取整个组织中对等活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 860bd71edf86a0cac8dcfb6e09bf5c587747f9c0
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980883"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="5adcc-104">Skype for Business 对等活动报表</span><span class="sxs-lookup"><span data-stu-id="5adcc-104">Skype for Business peer-to-peer activity reports</span></span>

<span data-ttu-id="5adcc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5adcc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5adcc-106">Skype for Business 对等活动报表可用于获取整个组织中对等活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5adcc-106">You can use the Skype for Business peer-to-peer activity reports to get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="5adcc-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="5adcc-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="5adcc-108">**注意：** 有关不同报告视图和名称的详细信息，请参阅 [Microsoft 365 报告 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="5adcc-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="5adcc-109">报告</span><span class="sxs-lookup"><span data-stu-id="5adcc-109">Reports</span></span>

| <span data-ttu-id="5adcc-110">函数</span><span class="sxs-lookup"><span data-stu-id="5adcc-110">Function</span></span>                                 | <span data-ttu-id="5adcc-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5adcc-111">Return Type</span></span> | <span data-ttu-id="5adcc-112">说明</span><span class="sxs-lookup"><span data-stu-id="5adcc-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="5adcc-113">获取活动计数</span><span class="sxs-lookup"><span data-stu-id="5adcc-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="5adcc-114">Stream</span><span class="sxs-lookup"><span data-stu-id="5adcc-114">Stream</span></span>      | <span data-ttu-id="5adcc-115">获取使用情况趋势，即组织中召开的会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="5adcc-115">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="5adcc-116">会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="5adcc-116">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="5adcc-117">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="5adcc-117">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="5adcc-118">Stream</span><span class="sxs-lookup"><span data-stu-id="5adcc-118">Stream</span></span>      | <span data-ttu-id="5adcc-119">获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="5adcc-119">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="5adcc-120">对等会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="5adcc-120">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="5adcc-121">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="5adcc-121">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="5adcc-122">Stream</span><span class="sxs-lookup"><span data-stu-id="5adcc-122">Stream</span></span>      | <span data-ttu-id="5adcc-123">获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="5adcc-123">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="5adcc-124">会话类型包括音频和视频。</span><span class="sxs-lookup"><span data-stu-id="5adcc-124">Types of sessions include audio and video.</span></span> |


