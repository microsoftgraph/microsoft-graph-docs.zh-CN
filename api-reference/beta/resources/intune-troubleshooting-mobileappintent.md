---
title: mobileAppIntent 枚举类型
description: 指示在设备上的移动应用程序的状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7cd26912406fc428f28c65abce2169c14d686342
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933377"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="9b4c5-103">mobileAppIntent 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9b4c5-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="9b4c5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9b4c5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b4c5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9b4c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b4c5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9b4c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b4c5-107">指示在设备上的移动应用程序的状态。</span><span class="sxs-lookup"><span data-stu-id="9b4c5-107">Indicates the status of the mobile app on the device.</span></span>
## <a name="members"></a><span data-ttu-id="9b4c5-108">成员</span><span class="sxs-lookup"><span data-stu-id="9b4c5-108">Members</span></span>
|<span data-ttu-id="9b4c5-109">成员</span><span class="sxs-lookup"><span data-stu-id="9b4c5-109">Member</span></span>|<span data-ttu-id="9b4c5-110">值</span><span class="sxs-lookup"><span data-stu-id="9b4c5-110">Value</span></span>|<span data-ttu-id="9b4c5-111">Description</span><span class="sxs-lookup"><span data-stu-id="9b4c5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b4c5-112">可用</span><span class="sxs-lookup"><span data-stu-id="9b4c5-112">available</span></span>|<span data-ttu-id="9b4c5-113">0</span><span class="sxs-lookup"><span data-stu-id="9b4c5-113">0</span></span>|<span data-ttu-id="9b4c5-114">可用</span><span class="sxs-lookup"><span data-stu-id="9b4c5-114">Available</span></span>|
|<span data-ttu-id="9b4c5-115">notAvailable</span><span class="sxs-lookup"><span data-stu-id="9b4c5-115">notAvailable</span></span>|<span data-ttu-id="9b4c5-116">1</span><span class="sxs-lookup"><span data-stu-id="9b4c5-116">1</span></span>|<span data-ttu-id="9b4c5-117">不可用</span><span class="sxs-lookup"><span data-stu-id="9b4c5-117">Not Available</span></span>|
|<span data-ttu-id="9b4c5-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="9b4c5-118">requiredInstall</span></span>|<span data-ttu-id="9b4c5-119">2</span><span class="sxs-lookup"><span data-stu-id="9b4c5-119">2</span></span>|<span data-ttu-id="9b4c5-120">所需的安装</span><span class="sxs-lookup"><span data-stu-id="9b4c5-120">Required Install</span></span>|
|<span data-ttu-id="9b4c5-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="9b4c5-121">requiredUninstall</span></span>|<span data-ttu-id="9b4c5-122">3</span><span class="sxs-lookup"><span data-stu-id="9b4c5-122">3</span></span>|<span data-ttu-id="9b4c5-123">需要的卸载</span><span class="sxs-lookup"><span data-stu-id="9b4c5-123">Required Uninstall</span></span>|
|<span data-ttu-id="9b4c5-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="9b4c5-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="9b4c5-125">4</span><span class="sxs-lookup"><span data-stu-id="9b4c5-125">4</span></span>|<span data-ttu-id="9b4c5-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="9b4c5-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="9b4c5-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="9b4c5-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="9b4c5-128">5</span><span class="sxs-lookup"><span data-stu-id="9b4c5-128">5</span></span>|<span data-ttu-id="9b4c5-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="9b4c5-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="9b4c5-130">排除</span><span class="sxs-lookup"><span data-stu-id="9b4c5-130">exclude</span></span>|<span data-ttu-id="9b4c5-131">6</span><span class="sxs-lookup"><span data-stu-id="9b4c5-131">6</span></span>|<span data-ttu-id="9b4c5-132">排除</span><span class="sxs-lookup"><span data-stu-id="9b4c5-132">Exclude</span></span>|





