---
title: Microsoft Teams 设备使用情况报告
description: '使用 Microsoft 团队设备使用率报告您的组织中获取的 Microsoft 团队设备用法见解。 '
localization_priority: Normal
ms.openlocfilehash: e89b5b133b8ebb64a59dfffe75ba9b47d2bf0c7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826157"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="49c3c-103">Microsoft Teams 设备使用情况报告</span><span class="sxs-lookup"><span data-stu-id="49c3c-103">Microsoft Teams device usage reports</span></span>

> <span data-ttu-id="49c3c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49c3c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49c3c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49c3c-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="49c3c-106">在 Microsoft Graph 中国由 21Vianet 不支持这些 Api。</span><span class="sxs-lookup"><span data-stu-id="49c3c-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="49c3c-107">使用 Microsoft 团队设备使用率报告您的组织中获取的 Microsoft 团队设备用法见解。</span><span class="sxs-lookup"><span data-stu-id="49c3c-107">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="49c3c-108">方法</span><span class="sxs-lookup"><span data-stu-id="49c3c-108">Methods</span></span>

| <span data-ttu-id="49c3c-109">方法</span><span class="sxs-lookup"><span data-stu-id="49c3c-109">Method</span></span>                                   | <span data-ttu-id="49c3c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="49c3c-110">Return Type</span></span>                              | <span data-ttu-id="49c3c-111">说明</span><span class="sxs-lookup"><span data-stu-id="49c3c-111">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="49c3c-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="49c3c-112">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="49c3c-113">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="49c3c-113">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="49c3c-114">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="49c3c-114">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="49c3c-115">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="49c3c-115">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="49c3c-116">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="49c3c-116">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="49c3c-117">按设备类型获取每日唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="49c3c-117">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="49c3c-118">获取分发用户计数</span><span class="sxs-lookup"><span data-stu-id="49c3c-118">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="49c3c-119">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="49c3c-119">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="49c3c-120">在选定的时间段内按设备类型获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="49c3c-120">Get the number of unique users by device type over the selected time period.</span></span> |
