---
title: Yammer 设备使用情况报表
description: Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: c23e67c22189ff08468b44b1993034616dd74e27
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070413"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="57ef2-104">Yammer 设备使用情况报表</span><span class="sxs-lookup"><span data-stu-id="57ef2-104">Yammer device usage reports</span></span>

<span data-ttu-id="57ef2-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57ef2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57ef2-106">Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。</span><span class="sxs-lookup"><span data-stu-id="57ef2-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="57ef2-107">可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。</span><span class="sxs-lookup"><span data-stu-id="57ef2-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="57ef2-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表-Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="57ef2-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="57ef2-109">报表</span><span class="sxs-lookup"><span data-stu-id="57ef2-109">Reports</span></span>

| <span data-ttu-id="57ef2-110">函数</span><span class="sxs-lookup"><span data-stu-id="57ef2-110">Function</span></span>                                 | <span data-ttu-id="57ef2-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="57ef2-111">CSV return type</span></span> | <span data-ttu-id="57ef2-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="57ef2-112">JSON return type</span></span>                         | <span data-ttu-id="57ef2-113">说明</span><span class="sxs-lookup"><span data-stu-id="57ef2-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="57ef2-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="57ef2-114">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="57ef2-115">Stream</span><span class="sxs-lookup"><span data-stu-id="57ef2-115">Stream</span></span>          | [<span data-ttu-id="57ef2-116">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="57ef2-116">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="57ef2-117">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="57ef2-117">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="57ef2-118">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="57ef2-118">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="57ef2-119">Stream</span><span class="sxs-lookup"><span data-stu-id="57ef2-119">Stream</span></span>          | [<span data-ttu-id="57ef2-120">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="57ef2-120">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="57ef2-121">按设备类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="57ef2-121">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="57ef2-122">获取用户数</span><span class="sxs-lookup"><span data-stu-id="57ef2-122">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="57ef2-123">Stream</span><span class="sxs-lookup"><span data-stu-id="57ef2-123">Stream</span></span>          | [<span data-ttu-id="57ef2-124">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="57ef2-124">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="57ef2-125">按设备类型获取每日用户数。</span><span class="sxs-lookup"><span data-stu-id="57ef2-125">Get the number of daily users by device type.</span></span> |


