---
title: Yammer 设备使用情况报表
description: Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f4736d92a990c94d2017cc8a26396a3cc4f6e04f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897748"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="55e09-104">Yammer 设备使用情况报表</span><span class="sxs-lookup"><span data-stu-id="55e09-104">Yammer device usage reports</span></span>

<span data-ttu-id="55e09-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55e09-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55e09-106">Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。</span><span class="sxs-lookup"><span data-stu-id="55e09-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="55e09-107">可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。</span><span class="sxs-lookup"><span data-stu-id="55e09-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="55e09-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="55e09-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="55e09-109">报表</span><span class="sxs-lookup"><span data-stu-id="55e09-109">Reports</span></span>

| <span data-ttu-id="55e09-110">函数</span><span class="sxs-lookup"><span data-stu-id="55e09-110">Function</span></span>                                 | <span data-ttu-id="55e09-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="55e09-111">Return Type</span></span> | <span data-ttu-id="55e09-112">说明</span><span class="sxs-lookup"><span data-stu-id="55e09-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="55e09-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="55e09-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="55e09-114">Stream</span><span class="sxs-lookup"><span data-stu-id="55e09-114">Stream</span></span>      | <span data-ttu-id="55e09-115">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="55e09-115">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="55e09-116">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="55e09-116">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="55e09-117">Stream</span><span class="sxs-lookup"><span data-stu-id="55e09-117">Stream</span></span>      | <span data-ttu-id="55e09-118">按设备类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="55e09-118">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="55e09-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="55e09-119">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="55e09-120">Stream</span><span class="sxs-lookup"><span data-stu-id="55e09-120">Stream</span></span>      | <span data-ttu-id="55e09-121">按设备类型获取每日用户数。</span><span class="sxs-lookup"><span data-stu-id="55e09-121">Get the number of daily users by device type.</span></span> |
