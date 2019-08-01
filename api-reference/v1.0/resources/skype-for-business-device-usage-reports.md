---
title: Skype for Business 设备使用情况报表
description: Skype for Business 设备使用情况报表可用于获取整个组织中使用的客户端和设备类型的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f84665f0840be87d14e2caafbeaa1d7edc8d6aa5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034116"
---
# <a name="skype-for-business-device-usage-reports"></a><span data-ttu-id="23996-104">Skype for Business 设备使用情况报表</span><span class="sxs-lookup"><span data-stu-id="23996-104">Skype for Business device usage reports</span></span>

<span data-ttu-id="23996-105">Skype for Business 设备使用情况报表可用于获取整个组织中使用的客户端和设备类型的详细信息。</span><span class="sxs-lookup"><span data-stu-id="23996-105">You can use the Skype for Business device usage reports to get details on the types of clients and devices that are used across your organization.</span></span> <span data-ttu-id="23996-106">为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。</span><span class="sxs-lookup"><span data-stu-id="23996-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="23996-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="23996-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="reports"></a><span data-ttu-id="23996-108">报表</span><span class="sxs-lookup"><span data-stu-id="23996-108">Reports</span></span>

| <span data-ttu-id="23996-109">函数</span><span class="sxs-lookup"><span data-stu-id="23996-109">Function</span></span>                                 | <span data-ttu-id="23996-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="23996-110">Return Type</span></span> | <span data-ttu-id="23996-111">说明</span><span class="sxs-lookup"><span data-stu-id="23996-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="23996-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="23996-112">Get user detail</span></span>](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="23996-113">流</span><span class="sxs-lookup"><span data-stu-id="23996-113">Stream</span></span>      | <span data-ttu-id="23996-114">获取用户的 Skype for Business 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="23996-114">Get details about Skype for Business device usage by user.</span></span> |
| [<span data-ttu-id="23996-115">获取分发用户数</span><span class="sxs-lookup"><span data-stu-id="23996-115">Get distribution user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="23996-116">Stream</span><span class="sxs-lookup"><span data-stu-id="23996-116">Stream</span></span>      | <span data-ttu-id="23996-117">获取组织中使用唯一设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="23996-117">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="23996-118">报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。</span><span class="sxs-lookup"><span data-stu-id="23996-118">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span> |
| [<span data-ttu-id="23996-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="23996-119">Get user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="23996-120">Stream</span><span class="sxs-lookup"><span data-stu-id="23996-120">Stream</span></span>      | <span data-ttu-id="23996-121">获取使用情况趋势，即组织中有多少用户已使用 Skype for Business 应用进行了连接。</span><span class="sxs-lookup"><span data-stu-id="23996-121">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="23996-122">还可以按设备类型（Windows、Windows 手机、Android 手机、iPhone 或 iPad）进一步了解整个组织中安装和使用的 Skype for Business 客户端应用。</span><span class="sxs-lookup"><span data-stu-id="23996-122">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span> |
