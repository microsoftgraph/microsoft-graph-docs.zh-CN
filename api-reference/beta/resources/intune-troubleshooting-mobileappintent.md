---
title: mobileAppIntent 枚举类型
description: 指示在设备上的移动应用程序的状态。
ms.openlocfilehash: 52d704f19379e2ac6232a37926185fd5d78c2e72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047293"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="a1031-103">mobileAppIntent 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a1031-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="a1031-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a1031-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1031-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a1031-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1031-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a1031-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1031-107">指示在设备上的移动应用程序的状态。</span><span class="sxs-lookup"><span data-stu-id="a1031-107">Indicates the status of the mobile app on the device.</span></span>
## <a name="members"></a><span data-ttu-id="a1031-108">成员</span><span class="sxs-lookup"><span data-stu-id="a1031-108">Members</span></span>
|<span data-ttu-id="a1031-109">成员</span><span class="sxs-lookup"><span data-stu-id="a1031-109">Member</span></span>|<span data-ttu-id="a1031-110">值</span><span class="sxs-lookup"><span data-stu-id="a1031-110">Value</span></span>|<span data-ttu-id="a1031-111">说明</span><span class="sxs-lookup"><span data-stu-id="a1031-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1031-112">可用</span><span class="sxs-lookup"><span data-stu-id="a1031-112">available</span></span>|<span data-ttu-id="a1031-113">0</span><span class="sxs-lookup"><span data-stu-id="a1031-113">0</span></span>|<span data-ttu-id="a1031-114">可用</span><span class="sxs-lookup"><span data-stu-id="a1031-114">Available</span></span>|
|<span data-ttu-id="a1031-115">notAvailable</span><span class="sxs-lookup"><span data-stu-id="a1031-115">notAvailable</span></span>|<span data-ttu-id="a1031-116">1</span><span class="sxs-lookup"><span data-stu-id="a1031-116">1</span></span>|<span data-ttu-id="a1031-117">不可用</span><span class="sxs-lookup"><span data-stu-id="a1031-117">Not Available</span></span>|
|<span data-ttu-id="a1031-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="a1031-118">requiredInstall</span></span>|<span data-ttu-id="a1031-119">2</span><span class="sxs-lookup"><span data-stu-id="a1031-119">2</span></span>|<span data-ttu-id="a1031-120">所需的安装</span><span class="sxs-lookup"><span data-stu-id="a1031-120">Required Install</span></span>|
|<span data-ttu-id="a1031-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="a1031-121">requiredUninstall</span></span>|<span data-ttu-id="a1031-122">3</span><span class="sxs-lookup"><span data-stu-id="a1031-122">3</span></span>|<span data-ttu-id="a1031-123">需要的卸载</span><span class="sxs-lookup"><span data-stu-id="a1031-123">Required Uninstall</span></span>|
|<span data-ttu-id="a1031-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="a1031-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="a1031-125">4</span><span class="sxs-lookup"><span data-stu-id="a1031-125">4</span></span>|<span data-ttu-id="a1031-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="a1031-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="a1031-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="a1031-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="a1031-128">5</span><span class="sxs-lookup"><span data-stu-id="a1031-128">5</span></span>|<span data-ttu-id="a1031-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="a1031-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="a1031-130">排除</span><span class="sxs-lookup"><span data-stu-id="a1031-130">exclude</span></span>|<span data-ttu-id="a1031-131">6</span><span class="sxs-lookup"><span data-stu-id="a1031-131">6</span></span>|<span data-ttu-id="a1031-132">排除</span><span class="sxs-lookup"><span data-stu-id="a1031-132">Exclude</span></span>|





