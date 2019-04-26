---
title: Yammer 设备使用情况报表
description: Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2c253d58d3f8b0bdd07d902bbcbe77af6a1666e9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342772"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="b1330-104">Yammer 设备使用情况报表</span><span class="sxs-lookup"><span data-stu-id="b1330-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1330-105">Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。</span><span class="sxs-lookup"><span data-stu-id="b1330-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="b1330-106">可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。</span><span class="sxs-lookup"><span data-stu-id="b1330-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="b1330-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="b1330-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="b1330-108">报表</span><span class="sxs-lookup"><span data-stu-id="b1330-108">Reports</span></span>

| <span data-ttu-id="b1330-109">函数</span><span class="sxs-lookup"><span data-stu-id="b1330-109">Function</span></span>                                 | <span data-ttu-id="b1330-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="b1330-110">CSV return type</span></span> | <span data-ttu-id="b1330-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="b1330-111">JSON return type</span></span>                         | <span data-ttu-id="b1330-112">说明</span><span class="sxs-lookup"><span data-stu-id="b1330-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="b1330-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="b1330-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="b1330-114">Stream</span><span class="sxs-lookup"><span data-stu-id="b1330-114">Stream</span></span>          | [<span data-ttu-id="b1330-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="b1330-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="b1330-116">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b1330-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="b1330-117">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="b1330-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="b1330-118">Stream</span><span class="sxs-lookup"><span data-stu-id="b1330-118">Stream</span></span>          | [<span data-ttu-id="b1330-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="b1330-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="b1330-120">按设备类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="b1330-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="b1330-121">获取用户数</span><span class="sxs-lookup"><span data-stu-id="b1330-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="b1330-122">Stream</span><span class="sxs-lookup"><span data-stu-id="b1330-122">Stream</span></span>          | [<span data-ttu-id="b1330-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="b1330-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="b1330-124">按设备类型获取每日用户数。</span><span class="sxs-lookup"><span data-stu-id="b1330-124">Get the number of daily users by device type.</span></span> |
