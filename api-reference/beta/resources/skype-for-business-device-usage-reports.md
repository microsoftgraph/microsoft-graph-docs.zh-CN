---
title: Skype for Business 设备使用情况报表
description: 你可以获取有关整个组织中使用的客户端和设备类型的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: da098fd702e9899c2d70cc1773b270d007ed356f
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983074"
---
# <a name="skype-for-business-device-usage-reports"></a><span data-ttu-id="f1e72-104">Skype for Business 设备使用情况报表</span><span class="sxs-lookup"><span data-stu-id="f1e72-104">Skype for Business device usage reports</span></span>

<span data-ttu-id="f1e72-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1e72-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1e72-106">你可以获取有关整个组织中使用的客户端和设备类型的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f1e72-106">You can get details on the types of clients and devices that are used across your organization.</span></span> <span data-ttu-id="f1e72-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="f1e72-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="f1e72-108">**注意：** 有关不同报告视图和名称的详细信息，请参阅 [Microsoft 365 报告 - 使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="f1e72-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="reports"></a><span data-ttu-id="f1e72-109">报告</span><span class="sxs-lookup"><span data-stu-id="f1e72-109">Reports</span></span>

| <span data-ttu-id="f1e72-110">函数</span><span class="sxs-lookup"><span data-stu-id="f1e72-110">Function</span></span>                                 | <span data-ttu-id="f1e72-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="f1e72-111">CSV return type</span></span> | <span data-ttu-id="f1e72-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="f1e72-112">JSON return type</span></span>                         | <span data-ttu-id="f1e72-113">说明</span><span class="sxs-lookup"><span data-stu-id="f1e72-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="f1e72-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="f1e72-114">Get user detail</span></span>](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="f1e72-115">Stream</span><span class="sxs-lookup"><span data-stu-id="f1e72-115">Stream</span></span>          | [<span data-ttu-id="f1e72-116">skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="f1e72-116">skypeForBusinessDeviceUsageUserDetail</span></span>](../resources/skypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="f1e72-117">获取用户的 Skype for Business 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f1e72-117">Get details about Skype for Business device usage by user.</span></span> |
| [<span data-ttu-id="f1e72-118">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="f1e72-118">Get distribution user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="f1e72-119">Stream</span><span class="sxs-lookup"><span data-stu-id="f1e72-119">Stream</span></span>          | [<span data-ttu-id="f1e72-120">skypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="f1e72-120">skypeForBusinessDeviceUsageDistributionUserCounts</span></span>](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="f1e72-121">获取组织中使用唯一设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="f1e72-121">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="f1e72-122">报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。</span><span class="sxs-lookup"><span data-stu-id="f1e72-122">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span> |
| [<span data-ttu-id="f1e72-123">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="f1e72-123">Get user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="f1e72-124">Stream</span><span class="sxs-lookup"><span data-stu-id="f1e72-124">Stream</span></span>          | [<span data-ttu-id="f1e72-125">skypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="f1e72-125">skypeForBusinessDeviceUsageUserCounts</span></span>](../resources/skypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="f1e72-126">获取使用情况趋势，即组织中有多少用户已使用 Skype for Business 应用进行了连接。</span><span class="sxs-lookup"><span data-stu-id="f1e72-126">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="f1e72-127">还可以按设备类型（Windows、Windows 手机、Android 手机、iPhone 或 iPad）进一步了解整个组织中安装和使用的 Skype for Business 客户端应用。</span><span class="sxs-lookup"><span data-stu-id="f1e72-127">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span> |


