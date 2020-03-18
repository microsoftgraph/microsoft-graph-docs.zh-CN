---
title: mobileAppIntent 枚举类型
description: 指示设备上的移动应用的状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7aa8da2d0cb32f641a050ae565568991b1b42ef4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42765081"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="8739d-103">mobileAppIntent 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8739d-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="8739d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8739d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8739d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8739d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8739d-106">指示设备上的移动应用的状态。</span><span class="sxs-lookup"><span data-stu-id="8739d-106">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="8739d-107">成员</span><span class="sxs-lookup"><span data-stu-id="8739d-107">Members</span></span>
|<span data-ttu-id="8739d-108">成员</span><span class="sxs-lookup"><span data-stu-id="8739d-108">Member</span></span>|<span data-ttu-id="8739d-109">值</span><span class="sxs-lookup"><span data-stu-id="8739d-109">Value</span></span>|<span data-ttu-id="8739d-110">说明</span><span class="sxs-lookup"><span data-stu-id="8739d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8739d-111">可用</span><span class="sxs-lookup"><span data-stu-id="8739d-111">available</span></span>|<span data-ttu-id="8739d-112">0</span><span class="sxs-lookup"><span data-stu-id="8739d-112">0</span></span>|<span data-ttu-id="8739d-113">可用</span><span class="sxs-lookup"><span data-stu-id="8739d-113">Available</span></span>|
|<span data-ttu-id="8739d-114">notAvailable</span><span class="sxs-lookup"><span data-stu-id="8739d-114">notAvailable</span></span>|<span data-ttu-id="8739d-115">1</span><span class="sxs-lookup"><span data-stu-id="8739d-115">1</span></span>|<span data-ttu-id="8739d-116">不可用</span><span class="sxs-lookup"><span data-stu-id="8739d-116">Not Available</span></span>|
|<span data-ttu-id="8739d-117">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="8739d-117">requiredInstall</span></span>|<span data-ttu-id="8739d-118">双面</span><span class="sxs-lookup"><span data-stu-id="8739d-118">2</span></span>|<span data-ttu-id="8739d-119">必需的安装</span><span class="sxs-lookup"><span data-stu-id="8739d-119">Required Install</span></span>|
|<span data-ttu-id="8739d-120">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="8739d-120">requiredUninstall</span></span>|<span data-ttu-id="8739d-121">第三章</span><span class="sxs-lookup"><span data-stu-id="8739d-121">3</span></span>|<span data-ttu-id="8739d-122">必需的卸载</span><span class="sxs-lookup"><span data-stu-id="8739d-122">Required Uninstall</span></span>|
|<span data-ttu-id="8739d-123">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="8739d-123">requiredAndAvailableInstall</span></span>|<span data-ttu-id="8739d-124">4 </span><span class="sxs-lookup"><span data-stu-id="8739d-124">4</span></span>|<span data-ttu-id="8739d-125">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="8739d-125">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="8739d-126">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="8739d-126">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="8739d-127">5 </span><span class="sxs-lookup"><span data-stu-id="8739d-127">5</span></span>|<span data-ttu-id="8739d-128">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="8739d-128">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="8739d-129">排除</span><span class="sxs-lookup"><span data-stu-id="8739d-129">exclude</span></span>|<span data-ttu-id="8739d-130">6 </span><span class="sxs-lookup"><span data-stu-id="8739d-130">6</span></span>|<span data-ttu-id="8739d-131">排除</span><span class="sxs-lookup"><span data-stu-id="8739d-131">Exclude</span></span>|



