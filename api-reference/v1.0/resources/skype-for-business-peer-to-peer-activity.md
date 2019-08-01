---
title: Skype for Business 对等活动报表
description: Skype for Business 对等活动报表可用于获取整个组织中对等活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 1bfab79ef77f0d92e47a9cabbd3c27d8cdcbbce6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034074"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="59df2-104">Skype for Business 对等活动报表</span><span class="sxs-lookup"><span data-stu-id="59df2-104">Skype for Business peer-to-peer activity reports</span></span>

<span data-ttu-id="59df2-105">Skype for Business 对等活动报表可用于获取整个组织中对等活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="59df2-105">You can use the Skype for Business peer-to-peer activity reports to get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="59df2-106">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="59df2-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="59df2-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="59df2-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="59df2-108">报表</span><span class="sxs-lookup"><span data-stu-id="59df2-108">Reports</span></span>

| <span data-ttu-id="59df2-109">函数</span><span class="sxs-lookup"><span data-stu-id="59df2-109">Function</span></span>                                 | <span data-ttu-id="59df2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="59df2-110">Return Type</span></span> | <span data-ttu-id="59df2-111">说明</span><span class="sxs-lookup"><span data-stu-id="59df2-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="59df2-112">获取活动数</span><span class="sxs-lookup"><span data-stu-id="59df2-112">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="59df2-113">流</span><span class="sxs-lookup"><span data-stu-id="59df2-113">Stream</span></span>      | <span data-ttu-id="59df2-114">获取使用情况趋势，即组织中召开的会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="59df2-114">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="59df2-115">会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="59df2-115">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="59df2-116">获取用户数</span><span class="sxs-lookup"><span data-stu-id="59df2-116">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="59df2-117">Stream</span><span class="sxs-lookup"><span data-stu-id="59df2-117">Stream</span></span>      | <span data-ttu-id="59df2-118">获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="59df2-118">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="59df2-119">对等会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="59df2-119">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="59df2-120">获取分钟数</span><span class="sxs-lookup"><span data-stu-id="59df2-120">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="59df2-121">Stream</span><span class="sxs-lookup"><span data-stu-id="59df2-121">Stream</span></span>      | <span data-ttu-id="59df2-122">获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="59df2-122">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="59df2-123">会话类型包括音频和视频。</span><span class="sxs-lookup"><span data-stu-id="59df2-123">Types of sessions include audio and video.</span></span> |

