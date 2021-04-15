---
title: Microsoft Teams 设备使用情况报告
description: '使用 Microsoft Teams 设备使用情况报告可深入了解贵组织的 Microsoft Teams 设备使用情况。 '
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: b9a4d2ab3034281970a3e342aa0a2d78e53678e5
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766110"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="3e14b-103">Microsoft Teams 设备使用情况报告</span><span class="sxs-lookup"><span data-stu-id="3e14b-103">Microsoft Teams device usage reports</span></span>

<span data-ttu-id="3e14b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e14b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e14b-105">使用 Microsoft Teams 设备使用情况报告可深入了解贵组织的 Microsoft Teams 设备使用情况。</span><span class="sxs-lookup"><span data-stu-id="3e14b-105">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="3e14b-106">方法</span><span class="sxs-lookup"><span data-stu-id="3e14b-106">Methods</span></span>

| <span data-ttu-id="3e14b-107">方法</span><span class="sxs-lookup"><span data-stu-id="3e14b-107">Method</span></span>                                                       | <span data-ttu-id="3e14b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3e14b-108">Return Type</span></span>                                                  | <span data-ttu-id="3e14b-109">说明</span><span class="sxs-lookup"><span data-stu-id="3e14b-109">Description</span></span>                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| [<span data-ttu-id="3e14b-110">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="3e14b-110">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="3e14b-111">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="3e14b-111">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="3e14b-112">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3e14b-112">Get details about Microsoft Teams device usage by user.</span></span>      |
| [<span data-ttu-id="3e14b-113">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="3e14b-113">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="3e14b-114">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="3e14b-114">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="3e14b-115">按设备类型获取每日唯一 Microsoft Teams 许可用户数。</span><span class="sxs-lookup"><span data-stu-id="3e14b-115">Get the number of daily unique Microsoft Teams licensed users by device type.</span></span> |
| [<span data-ttu-id="3e14b-116">获取用户总数</span><span class="sxs-lookup"><span data-stu-id="3e14b-116">Get total user counts</span></span>](../api/reportroot-getteamsdeviceusagetotalusercounts.md) | [<span data-ttu-id="3e14b-117">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="3e14b-117">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="3e14b-118">按设备类型获取每日唯一 Microsoft Teams 许可或非许可用户的数量。</span><span class="sxs-lookup"><span data-stu-id="3e14b-118">Get the number of daily unique Microsoft Teams licensed or non-licensed users by device type.</span></span> |
| [<span data-ttu-id="3e14b-119">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="3e14b-119">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="3e14b-120">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="3e14b-120">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="3e14b-121">按设备类型获取选定时段内唯一 Microsoft Teams 许可用户的数量。</span><span class="sxs-lookup"><span data-stu-id="3e14b-121">Get the number of unique Microsoft Teams licensed users by device type over the selected time period.</span></span> |
| [<span data-ttu-id="3e14b-122">获取分发用户总数</span><span class="sxs-lookup"><span data-stu-id="3e14b-122">Get distribution total user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributiontotalusercounts.md) | [<span data-ttu-id="3e14b-123">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="3e14b-123">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="3e14b-124">按设备类型获取选定时段内唯一 Microsoft Teams 许可或非许可用户的数量。</span><span class="sxs-lookup"><span data-stu-id="3e14b-124">Get the number of unique Microsoft Teams licensed or non-licensed users by device type over the selected time period.</span></span> |


