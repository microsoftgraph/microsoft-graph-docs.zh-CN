---
title: mobileAppIntent 枚举类型
description: 指示设备上的移动应用的状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1ea3de0799c31e18603661ef081fc03a0146f341
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43317835"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="10ca7-103">mobileAppIntent 枚举类型</span><span class="sxs-lookup"><span data-stu-id="10ca7-103">mobileAppIntent enum type</span></span>

<span data-ttu-id="10ca7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10ca7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10ca7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10ca7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10ca7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10ca7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10ca7-107">指示设备上的移动应用的状态。</span><span class="sxs-lookup"><span data-stu-id="10ca7-107">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="10ca7-108">成员</span><span class="sxs-lookup"><span data-stu-id="10ca7-108">Members</span></span>
|<span data-ttu-id="10ca7-109">成员</span><span class="sxs-lookup"><span data-stu-id="10ca7-109">Member</span></span>|<span data-ttu-id="10ca7-110">值</span><span class="sxs-lookup"><span data-stu-id="10ca7-110">Value</span></span>|<span data-ttu-id="10ca7-111">说明</span><span class="sxs-lookup"><span data-stu-id="10ca7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10ca7-112">可用</span><span class="sxs-lookup"><span data-stu-id="10ca7-112">available</span></span>|<span data-ttu-id="10ca7-113">0</span><span class="sxs-lookup"><span data-stu-id="10ca7-113">0</span></span>|<span data-ttu-id="10ca7-114">可用</span><span class="sxs-lookup"><span data-stu-id="10ca7-114">Available</span></span>|
|<span data-ttu-id="10ca7-115">notAvailable</span><span class="sxs-lookup"><span data-stu-id="10ca7-115">notAvailable</span></span>|<span data-ttu-id="10ca7-116">1</span><span class="sxs-lookup"><span data-stu-id="10ca7-116">1</span></span>|<span data-ttu-id="10ca7-117">不可用</span><span class="sxs-lookup"><span data-stu-id="10ca7-117">Not Available</span></span>|
|<span data-ttu-id="10ca7-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="10ca7-118">requiredInstall</span></span>|<span data-ttu-id="10ca7-119">双面</span><span class="sxs-lookup"><span data-stu-id="10ca7-119">2</span></span>|<span data-ttu-id="10ca7-120">必需的安装</span><span class="sxs-lookup"><span data-stu-id="10ca7-120">Required Install</span></span>|
|<span data-ttu-id="10ca7-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="10ca7-121">requiredUninstall</span></span>|<span data-ttu-id="10ca7-122">第三章</span><span class="sxs-lookup"><span data-stu-id="10ca7-122">3</span></span>|<span data-ttu-id="10ca7-123">必需的卸载</span><span class="sxs-lookup"><span data-stu-id="10ca7-123">Required Uninstall</span></span>|
|<span data-ttu-id="10ca7-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="10ca7-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="10ca7-125">4 </span><span class="sxs-lookup"><span data-stu-id="10ca7-125">4</span></span>|<span data-ttu-id="10ca7-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="10ca7-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="10ca7-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="10ca7-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="10ca7-128">5 </span><span class="sxs-lookup"><span data-stu-id="10ca7-128">5</span></span>|<span data-ttu-id="10ca7-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="10ca7-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="10ca7-130">排除</span><span class="sxs-lookup"><span data-stu-id="10ca7-130">exclude</span></span>|<span data-ttu-id="10ca7-131">6 </span><span class="sxs-lookup"><span data-stu-id="10ca7-131">6</span></span>|<span data-ttu-id="10ca7-132">排除</span><span class="sxs-lookup"><span data-stu-id="10ca7-132">Exclude</span></span>|



