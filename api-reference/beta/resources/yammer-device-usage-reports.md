---
title: Yammer 设备使用情况报表
description: Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a68b1decf0690a07db07c880cec25a1bf2c01cfa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991956"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="95693-104">Yammer 设备使用情况报表</span><span class="sxs-lookup"><span data-stu-id="95693-104">Yammer device usage reports</span></span>

> <span data-ttu-id="95693-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="95693-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95693-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="95693-106">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="95693-107">在 Microsoft Graph 中国由 21Vianet 不支持这些 Api。</span><span class="sxs-lookup"><span data-stu-id="95693-107">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="95693-108">Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。</span><span class="sxs-lookup"><span data-stu-id="95693-108">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="95693-109">可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。</span><span class="sxs-lookup"><span data-stu-id="95693-109">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="95693-110">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="95693-110">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="95693-111">报表</span><span class="sxs-lookup"><span data-stu-id="95693-111">Reports</span></span>

| <span data-ttu-id="95693-112">函数</span><span class="sxs-lookup"><span data-stu-id="95693-112">Function</span></span>                                 | <span data-ttu-id="95693-113">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="95693-113">CSV return type</span></span> | <span data-ttu-id="95693-114">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="95693-114">JSON return type</span></span>                         | <span data-ttu-id="95693-115">说明</span><span class="sxs-lookup"><span data-stu-id="95693-115">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="95693-116">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="95693-116">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="95693-117">Stream</span><span class="sxs-lookup"><span data-stu-id="95693-117">Stream</span></span>          | [<span data-ttu-id="95693-118">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="95693-118">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="95693-119">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="95693-119">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="95693-120">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="95693-120">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="95693-121">Stream</span><span class="sxs-lookup"><span data-stu-id="95693-121">Stream</span></span>          | [<span data-ttu-id="95693-122">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="95693-122">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="95693-123">按设备类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="95693-123">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="95693-124">获取用户数</span><span class="sxs-lookup"><span data-stu-id="95693-124">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="95693-125">Stream</span><span class="sxs-lookup"><span data-stu-id="95693-125">Stream</span></span>          | [<span data-ttu-id="95693-126">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="95693-126">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="95693-127">按设备类型获取每日用户数。</span><span class="sxs-lookup"><span data-stu-id="95693-127">Get the number of daily users by device type.</span></span> |
