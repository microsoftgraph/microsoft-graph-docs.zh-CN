---
title: mobileAppIntent 枚举类型
description: 指示设备上的移动应用的状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 472fd157ed26b8b446e272d37baa135584cbbe0b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785914"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="d3743-103">mobileAppIntent 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d3743-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="d3743-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3743-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3743-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3743-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3743-106">指示设备上的移动应用的状态。</span><span class="sxs-lookup"><span data-stu-id="d3743-106">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="d3743-107">成员</span><span class="sxs-lookup"><span data-stu-id="d3743-107">Members</span></span>
|<span data-ttu-id="d3743-108">成员</span><span class="sxs-lookup"><span data-stu-id="d3743-108">Member</span></span>|<span data-ttu-id="d3743-109">值</span><span class="sxs-lookup"><span data-stu-id="d3743-109">Value</span></span>|<span data-ttu-id="d3743-110">说明</span><span class="sxs-lookup"><span data-stu-id="d3743-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3743-111">可用</span><span class="sxs-lookup"><span data-stu-id="d3743-111">available</span></span>|<span data-ttu-id="d3743-112">0</span><span class="sxs-lookup"><span data-stu-id="d3743-112">0</span></span>|<span data-ttu-id="d3743-113">可用</span><span class="sxs-lookup"><span data-stu-id="d3743-113">Available</span></span>|
|<span data-ttu-id="d3743-114">notAvailable</span><span class="sxs-lookup"><span data-stu-id="d3743-114">notAvailable</span></span>|<span data-ttu-id="d3743-115">1</span><span class="sxs-lookup"><span data-stu-id="d3743-115">1</span></span>|<span data-ttu-id="d3743-116">不可用</span><span class="sxs-lookup"><span data-stu-id="d3743-116">Not Available</span></span>|
|<span data-ttu-id="d3743-117">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="d3743-117">requiredInstall</span></span>|<span data-ttu-id="d3743-118">双面</span><span class="sxs-lookup"><span data-stu-id="d3743-118">2</span></span>|<span data-ttu-id="d3743-119">必需的安装</span><span class="sxs-lookup"><span data-stu-id="d3743-119">Required Install</span></span>|
|<span data-ttu-id="d3743-120">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="d3743-120">requiredUninstall</span></span>|<span data-ttu-id="d3743-121">第三章</span><span class="sxs-lookup"><span data-stu-id="d3743-121">3</span></span>|<span data-ttu-id="d3743-122">必需的卸载</span><span class="sxs-lookup"><span data-stu-id="d3743-122">Required Uninstall</span></span>|
|<span data-ttu-id="d3743-123">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="d3743-123">requiredAndAvailableInstall</span></span>|<span data-ttu-id="d3743-124">4</span><span class="sxs-lookup"><span data-stu-id="d3743-124">4</span></span>|<span data-ttu-id="d3743-125">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="d3743-125">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="d3743-126">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="d3743-126">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="d3743-127">5</span><span class="sxs-lookup"><span data-stu-id="d3743-127">5</span></span>|<span data-ttu-id="d3743-128">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="d3743-128">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="d3743-129">排除</span><span class="sxs-lookup"><span data-stu-id="d3743-129">exclude</span></span>|<span data-ttu-id="d3743-130">型</span><span class="sxs-lookup"><span data-stu-id="d3743-130">6</span></span>|<span data-ttu-id="d3743-131">排除</span><span class="sxs-lookup"><span data-stu-id="d3743-131">Exclude</span></span>|



