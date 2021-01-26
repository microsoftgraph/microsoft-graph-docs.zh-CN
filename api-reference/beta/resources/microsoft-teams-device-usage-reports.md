---
title: Microsoft Teams 设备使用情况报告
description: '使用 Microsoft Teams 设备使用情况报告深入了解组织中 Microsoft Teams 设备使用情况。 '
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7be5d8d0d369d9cff0fe295f8765a5e4f3ca28bc
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980786"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="be241-103">Microsoft Teams 设备使用情况报告</span><span class="sxs-lookup"><span data-stu-id="be241-103">Microsoft Teams device usage reports</span></span>

<span data-ttu-id="be241-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be241-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be241-105">使用 Microsoft Teams 设备使用情况报告深入了解组织中 Microsoft Teams 设备使用情况。</span><span class="sxs-lookup"><span data-stu-id="be241-105">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="be241-106">方法</span><span class="sxs-lookup"><span data-stu-id="be241-106">Methods</span></span>

| <span data-ttu-id="be241-107">方法</span><span class="sxs-lookup"><span data-stu-id="be241-107">Method</span></span>                                   | <span data-ttu-id="be241-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="be241-108">Return Type</span></span>                              | <span data-ttu-id="be241-109">说明</span><span class="sxs-lookup"><span data-stu-id="be241-109">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="be241-110">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="be241-110">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="be241-111">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="be241-111">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="be241-112">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="be241-112">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="be241-113">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="be241-113">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="be241-114">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="be241-114">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="be241-115">按设备类型获取每日唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="be241-115">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="be241-116">获取分发用户计数</span><span class="sxs-lookup"><span data-stu-id="be241-116">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="be241-117">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="be241-117">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="be241-118">在选定的时间段内按设备类型获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="be241-118">Get the number of unique users by device type over the selected time period.</span></span> |


