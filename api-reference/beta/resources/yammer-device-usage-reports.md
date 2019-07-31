---
title: Yammer 设备使用情况报表
description: Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f36ed78805bc664adfbbd4ced9bc86b1444ab262
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007002"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="7d13e-104">Yammer 设备使用情况报表</span><span class="sxs-lookup"><span data-stu-id="7d13e-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d13e-105">Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。</span><span class="sxs-lookup"><span data-stu-id="7d13e-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="7d13e-106">可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。</span><span class="sxs-lookup"><span data-stu-id="7d13e-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="7d13e-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="7d13e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="7d13e-108">报表</span><span class="sxs-lookup"><span data-stu-id="7d13e-108">Reports</span></span>

| <span data-ttu-id="7d13e-109">函数</span><span class="sxs-lookup"><span data-stu-id="7d13e-109">Function</span></span>                                 | <span data-ttu-id="7d13e-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="7d13e-110">CSV return type</span></span> | <span data-ttu-id="7d13e-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="7d13e-111">JSON return type</span></span>                         | <span data-ttu-id="7d13e-112">说明</span><span class="sxs-lookup"><span data-stu-id="7d13e-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="7d13e-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="7d13e-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="7d13e-114">流</span><span class="sxs-lookup"><span data-stu-id="7d13e-114">Stream</span></span>          | [<span data-ttu-id="7d13e-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="7d13e-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="7d13e-116">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7d13e-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="7d13e-117">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="7d13e-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="7d13e-118">Stream</span><span class="sxs-lookup"><span data-stu-id="7d13e-118">Stream</span></span>          | [<span data-ttu-id="7d13e-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="7d13e-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="7d13e-120">按设备类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="7d13e-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="7d13e-121">获取用户数</span><span class="sxs-lookup"><span data-stu-id="7d13e-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="7d13e-122">Stream</span><span class="sxs-lookup"><span data-stu-id="7d13e-122">Stream</span></span>          | [<span data-ttu-id="7d13e-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="7d13e-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="7d13e-124">按设备类型获取每日用户数。</span><span class="sxs-lookup"><span data-stu-id="7d13e-124">Get the number of daily users by device type.</span></span> |
