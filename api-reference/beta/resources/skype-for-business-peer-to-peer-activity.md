---
title: Skype for Business 对等活动报表
description: 你可以在组织中获取对等活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 6787fac69adfdd4a5af7c6d8ae0b87b2213b636d
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896488"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="bd99f-104">Skype for Business 对等活动报表</span><span class="sxs-lookup"><span data-stu-id="bd99f-104">Skype for Business peer-to-peer activity reports</span></span>

<span data-ttu-id="bd99f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd99f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd99f-106">你可以在组织中获取对等活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bd99f-106">You can get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="bd99f-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="bd99f-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="bd99f-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-Skype For business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="bd99f-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="bd99f-109">报表</span><span class="sxs-lookup"><span data-stu-id="bd99f-109">Reports</span></span>

| <span data-ttu-id="bd99f-110">函数</span><span class="sxs-lookup"><span data-stu-id="bd99f-110">Function</span></span>                                 | <span data-ttu-id="bd99f-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="bd99f-111">CSV return type</span></span> | <span data-ttu-id="bd99f-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="bd99f-112">JSON return type</span></span>                         | <span data-ttu-id="bd99f-113">说明</span><span class="sxs-lookup"><span data-stu-id="bd99f-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="bd99f-114">获取活动数</span><span class="sxs-lookup"><span data-stu-id="bd99f-114">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="bd99f-115">Stream</span><span class="sxs-lookup"><span data-stu-id="bd99f-115">Stream</span></span>          | [<span data-ttu-id="bd99f-116">skypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="bd99f-116">skypeForBusinessPeerToPeerActivityCounts</span></span>](../resources/skypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="bd99f-117">获取使用情况趋势，即组织中召开的会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="bd99f-117">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="bd99f-118">会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="bd99f-118">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="bd99f-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="bd99f-119">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="bd99f-120">Stream</span><span class="sxs-lookup"><span data-stu-id="bd99f-120">Stream</span></span>          | [<span data-ttu-id="bd99f-121">skypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="bd99f-121">skypeForBusinessPeerToPeerActivityUserCounts</span></span>](../resources/skypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="bd99f-122">获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="bd99f-122">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="bd99f-123">对等会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="bd99f-123">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="bd99f-124">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="bd99f-124">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="bd99f-125">Stream</span><span class="sxs-lookup"><span data-stu-id="bd99f-125">Stream</span></span>          | [<span data-ttu-id="bd99f-126">skypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="bd99f-126">skypeForBusinessPeerToPeerActivityMinuteCounts</span></span>](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="bd99f-127">获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="bd99f-127">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="bd99f-128">会话类型包括音频和视频。</span><span class="sxs-lookup"><span data-stu-id="bd99f-128">Types of sessions include audio and video.</span></span> |
