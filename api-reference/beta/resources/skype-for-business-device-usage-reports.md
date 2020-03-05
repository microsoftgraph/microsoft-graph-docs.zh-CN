---
title: Skype for Business 设备使用情况报表
description: 您可以获取有关在组织中使用的客户端和设备的类型的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 6a006f04d710e7d7b210cb55e72a0418bdf124d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520483"
---
# <a name="skype-for-business-device-usage-reports"></a><span data-ttu-id="53220-104">Skype for Business 设备使用情况报表</span><span class="sxs-lookup"><span data-stu-id="53220-104">Skype for Business device usage reports</span></span>

<span data-ttu-id="53220-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="53220-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53220-106">您可以获取有关在组织中使用的客户端和设备的类型的详细信息。</span><span class="sxs-lookup"><span data-stu-id="53220-106">You can get details on the types of clients and devices that are used across your organization.</span></span> <span data-ttu-id="53220-107">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="53220-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="53220-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="53220-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="reports"></a><span data-ttu-id="53220-109">报表</span><span class="sxs-lookup"><span data-stu-id="53220-109">Reports</span></span>

| <span data-ttu-id="53220-110">函数</span><span class="sxs-lookup"><span data-stu-id="53220-110">Function</span></span>                                 | <span data-ttu-id="53220-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="53220-111">CSV return type</span></span> | <span data-ttu-id="53220-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="53220-112">JSON return type</span></span>                         | <span data-ttu-id="53220-113">说明</span><span class="sxs-lookup"><span data-stu-id="53220-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="53220-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="53220-114">Get user detail</span></span>](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="53220-115">Stream</span><span class="sxs-lookup"><span data-stu-id="53220-115">Stream</span></span>          | [<span data-ttu-id="53220-116">skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="53220-116">skypeForBusinessDeviceUsageUserDetail</span></span>](../resources/skypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="53220-117">获取用户的 Skype for Business 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="53220-117">Get details about Skype for Business device usage by user.</span></span> |
| [<span data-ttu-id="53220-118">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="53220-118">Get distribution user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="53220-119">Stream</span><span class="sxs-lookup"><span data-stu-id="53220-119">Stream</span></span>          | [<span data-ttu-id="53220-120">skypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="53220-120">skypeForBusinessDeviceUsageDistributionUserCounts</span></span>](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="53220-121">获取组织中使用唯一设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="53220-121">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="53220-122">报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。</span><span class="sxs-lookup"><span data-stu-id="53220-122">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span> |
| [<span data-ttu-id="53220-123">获取用户数</span><span class="sxs-lookup"><span data-stu-id="53220-123">Get user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="53220-124">Stream</span><span class="sxs-lookup"><span data-stu-id="53220-124">Stream</span></span>          | [<span data-ttu-id="53220-125">skypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="53220-125">skypeForBusinessDeviceUsageUserCounts</span></span>](../resources/skypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="53220-126">获取使用情况趋势，即组织中有多少用户已使用 Skype for Business 应用进行了连接。</span><span class="sxs-lookup"><span data-stu-id="53220-126">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="53220-127">还可以按设备类型（Windows、Windows 手机、Android 手机、iPhone 或 iPad）进一步了解整个组织中安装和使用的 Skype for Business 客户端应用。</span><span class="sxs-lookup"><span data-stu-id="53220-127">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span> |
