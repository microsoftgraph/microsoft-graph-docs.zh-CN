---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5869bcfaa3949a8463d2625c4e7de48897a62daf
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943604"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="247e4-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="247e4-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="247e4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="247e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="247e4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="247e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="247e4-106">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="247e4-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="247e4-107">成员</span><span class="sxs-lookup"><span data-stu-id="247e4-107">Members</span></span>
|<span data-ttu-id="247e4-108">成员</span><span class="sxs-lookup"><span data-stu-id="247e4-108">Member</span></span>|<span data-ttu-id="247e4-109">值</span><span class="sxs-lookup"><span data-stu-id="247e4-109">Value</span></span>|<span data-ttu-id="247e4-110">说明</span><span class="sxs-lookup"><span data-stu-id="247e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="247e4-111">定制</span><span class="sxs-lookup"><span data-stu-id="247e4-111">userDefined</span></span>|<span data-ttu-id="247e4-112">0</span><span class="sxs-lookup"><span data-stu-id="247e4-112">0</span></span>|<span data-ttu-id="247e4-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="247e4-113">Allow the user to set.</span></span>|
|<span data-ttu-id="247e4-114">各种</span><span class="sxs-lookup"><span data-stu-id="247e4-114">all</span></span>|<span data-ttu-id="247e4-115">1</span><span class="sxs-lookup"><span data-stu-id="247e4-115">1</span></span>|<span data-ttu-id="247e4-116">半年频道 (定向)。</span><span class="sxs-lookup"><span data-stu-id="247e4-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="247e4-117">设备从半年频道 (定向) 获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="247e4-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="247e4-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="247e4-118">businessReadyOnly</span></span>|<span data-ttu-id="247e4-119">双面</span><span class="sxs-lookup"><span data-stu-id="247e4-119">2</span></span>|<span data-ttu-id="247e4-120">半年频道。</span><span class="sxs-lookup"><span data-stu-id="247e4-120">Semi-annual Channel.</span></span> <span data-ttu-id="247e4-121">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="247e4-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="247e4-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="247e4-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="247e4-123">第三章</span><span class="sxs-lookup"><span data-stu-id="247e4-123">3</span></span>|<span data-ttu-id="247e4-124">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="247e4-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="247e4-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="247e4-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="247e4-126">4</span><span class="sxs-lookup"><span data-stu-id="247e4-126">4</span></span>|<span data-ttu-id="247e4-127">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="247e4-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="247e4-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="247e4-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="247e4-129">5</span><span class="sxs-lookup"><span data-stu-id="247e4-129">5</span></span>|<span data-ttu-id="247e4-130">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="247e4-130">Release Windows Insider build</span></span>|




