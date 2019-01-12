---
title: Microsoft Teams 设备使用情况报告
description: '使用 Microsoft 团队设备使用率报告您的组织中获取的 Microsoft 团队设备用法见解。 '
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2320b997ddc4bb9fb39ef528eecaca8a7c452426
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931030"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="e8ada-103">Microsoft Teams 设备使用情况报告</span><span class="sxs-lookup"><span data-stu-id="e8ada-103">Microsoft Teams device usage reports</span></span>

> <span data-ttu-id="e8ada-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8ada-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8ada-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8ada-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="e8ada-106">在 Microsoft Graph 中国由 21Vianet 不支持这些 Api。</span><span class="sxs-lookup"><span data-stu-id="e8ada-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="e8ada-107">使用 Microsoft 团队设备使用率报告您的组织中获取的 Microsoft 团队设备用法见解。</span><span class="sxs-lookup"><span data-stu-id="e8ada-107">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="e8ada-108">方法</span><span class="sxs-lookup"><span data-stu-id="e8ada-108">Methods</span></span>

| <span data-ttu-id="e8ada-109">方法</span><span class="sxs-lookup"><span data-stu-id="e8ada-109">Method</span></span>                                   | <span data-ttu-id="e8ada-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e8ada-110">Return Type</span></span>                              | <span data-ttu-id="e8ada-111">说明</span><span class="sxs-lookup"><span data-stu-id="e8ada-111">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="e8ada-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="e8ada-112">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="e8ada-113">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="e8ada-113">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="e8ada-114">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e8ada-114">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="e8ada-115">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="e8ada-115">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="e8ada-116">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="e8ada-116">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="e8ada-117">按设备类型获取每日唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="e8ada-117">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="e8ada-118">获取分发用户计数</span><span class="sxs-lookup"><span data-stu-id="e8ada-118">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="e8ada-119">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="e8ada-119">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="e8ada-120">在选定的时间段内按设备类型获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="e8ada-120">Get the number of unique users by device type over the selected time period.</span></span> |
