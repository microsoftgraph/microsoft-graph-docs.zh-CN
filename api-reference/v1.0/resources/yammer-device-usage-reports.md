---
title: Yammer 设备使用情况报表
description: Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 3e2c91db77fbd57118c340d2d51a3bcd67ac0641
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446637"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="88da2-104">Yammer 设备使用情况报表</span><span class="sxs-lookup"><span data-stu-id="88da2-104">Yammer device usage reports</span></span>

<span data-ttu-id="88da2-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="88da2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88da2-106">Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。</span><span class="sxs-lookup"><span data-stu-id="88da2-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="88da2-107">可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。</span><span class="sxs-lookup"><span data-stu-id="88da2-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="88da2-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="88da2-108">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="88da2-109">报表</span><span class="sxs-lookup"><span data-stu-id="88da2-109">Reports</span></span>

| <span data-ttu-id="88da2-110">函数</span><span class="sxs-lookup"><span data-stu-id="88da2-110">Function</span></span>                                 | <span data-ttu-id="88da2-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="88da2-111">Return Type</span></span> | <span data-ttu-id="88da2-112">说明</span><span class="sxs-lookup"><span data-stu-id="88da2-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="88da2-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="88da2-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="88da2-114">Stream</span><span class="sxs-lookup"><span data-stu-id="88da2-114">Stream</span></span>      | <span data-ttu-id="88da2-115">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="88da2-115">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="88da2-116">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="88da2-116">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="88da2-117">Stream</span><span class="sxs-lookup"><span data-stu-id="88da2-117">Stream</span></span>      | <span data-ttu-id="88da2-118">按设备类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="88da2-118">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="88da2-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="88da2-119">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="88da2-120">Stream</span><span class="sxs-lookup"><span data-stu-id="88da2-120">Stream</span></span>      | <span data-ttu-id="88da2-121">按设备类型获取每日用户数。</span><span class="sxs-lookup"><span data-stu-id="88da2-121">Get the number of daily users by device type.</span></span> |
