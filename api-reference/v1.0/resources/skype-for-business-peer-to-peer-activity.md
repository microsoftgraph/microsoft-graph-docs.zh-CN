---
title: Skype for Business 对等活动报表
description: Skype for Business 对等活动报表可用于获取整个组织中对等活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 5d967cd8a150d70598a98fd9019087472216a296
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970549"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="75e8c-104">Skype for Business 对等活动报表</span><span class="sxs-lookup"><span data-stu-id="75e8c-104">Skype for Business peer-to-peer activity reports</span></span>

<span data-ttu-id="75e8c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75e8c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75e8c-106">Skype for Business 对等活动报表可用于获取整个组织中对等活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="75e8c-106">You can use the Skype for Business peer-to-peer activity reports to get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="75e8c-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="75e8c-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="75e8c-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 reports-Skype For business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="75e8c-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="75e8c-109">报表</span><span class="sxs-lookup"><span data-stu-id="75e8c-109">Reports</span></span>

| <span data-ttu-id="75e8c-110">函数</span><span class="sxs-lookup"><span data-stu-id="75e8c-110">Function</span></span>                                 | <span data-ttu-id="75e8c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="75e8c-111">Return Type</span></span> | <span data-ttu-id="75e8c-112">说明</span><span class="sxs-lookup"><span data-stu-id="75e8c-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="75e8c-113">获取活动数</span><span class="sxs-lookup"><span data-stu-id="75e8c-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="75e8c-114">Stream</span><span class="sxs-lookup"><span data-stu-id="75e8c-114">Stream</span></span>      | <span data-ttu-id="75e8c-115">获取使用情况趋势，即组织中召开的会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="75e8c-115">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="75e8c-116">会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="75e8c-116">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="75e8c-117">获取用户数</span><span class="sxs-lookup"><span data-stu-id="75e8c-117">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="75e8c-118">Stream</span><span class="sxs-lookup"><span data-stu-id="75e8c-118">Stream</span></span>      | <span data-ttu-id="75e8c-119">获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="75e8c-119">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="75e8c-120">对等会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="75e8c-120">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="75e8c-121">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="75e8c-121">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="75e8c-122">Stream</span><span class="sxs-lookup"><span data-stu-id="75e8c-122">Stream</span></span>      | <span data-ttu-id="75e8c-123">获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="75e8c-123">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="75e8c-124">会话类型包括音频和视频。</span><span class="sxs-lookup"><span data-stu-id="75e8c-124">Types of sessions include audio and video.</span></span> |


