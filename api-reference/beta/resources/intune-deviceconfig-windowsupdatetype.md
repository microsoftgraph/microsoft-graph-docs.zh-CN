---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17aad82b25982b90ecea348d959e2ed2ec94a483
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169158"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="bb4c6-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bb4c6-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="bb4c6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb4c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb4c6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb4c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb4c6-106">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="bb4c6-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="bb4c6-107">成员</span><span class="sxs-lookup"><span data-stu-id="bb4c6-107">Members</span></span>
|<span data-ttu-id="bb4c6-108">成员</span><span class="sxs-lookup"><span data-stu-id="bb4c6-108">Member</span></span>|<span data-ttu-id="bb4c6-109">值</span><span class="sxs-lookup"><span data-stu-id="bb4c6-109">Value</span></span>|<span data-ttu-id="bb4c6-110">说明</span><span class="sxs-lookup"><span data-stu-id="bb4c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb4c6-111">定制</span><span class="sxs-lookup"><span data-stu-id="bb4c6-111">userDefined</span></span>|<span data-ttu-id="bb4c6-112">0</span><span class="sxs-lookup"><span data-stu-id="bb4c6-112">0</span></span>|<span data-ttu-id="bb4c6-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="bb4c6-113">Allow the user to set.</span></span>|
|<span data-ttu-id="bb4c6-114">all</span><span class="sxs-lookup"><span data-stu-id="bb4c6-114">all</span></span>|<span data-ttu-id="bb4c6-115">1</span><span class="sxs-lookup"><span data-stu-id="bb4c6-115">1</span></span>|<span data-ttu-id="bb4c6-116">半年频道 (定向)。</span><span class="sxs-lookup"><span data-stu-id="bb4c6-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="bb4c6-117">设备从半年频道 (定向) 获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="bb4c6-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="bb4c6-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="bb4c6-118">businessReadyOnly</span></span>|<span data-ttu-id="bb4c6-119">双面</span><span class="sxs-lookup"><span data-stu-id="bb4c6-119">2</span></span>|<span data-ttu-id="bb4c6-120">半年频道。</span><span class="sxs-lookup"><span data-stu-id="bb4c6-120">Semi-annual Channel.</span></span> <span data-ttu-id="bb4c6-121">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="bb4c6-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="bb4c6-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="bb4c6-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="bb4c6-123">第三章</span><span class="sxs-lookup"><span data-stu-id="bb4c6-123">3</span></span>|<span data-ttu-id="bb4c6-124">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="bb4c6-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="bb4c6-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="bb4c6-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="bb4c6-126">4</span><span class="sxs-lookup"><span data-stu-id="bb4c6-126">4</span></span>|<span data-ttu-id="bb4c6-127">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="bb4c6-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="bb4c6-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="bb4c6-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="bb4c6-129">5</span><span class="sxs-lookup"><span data-stu-id="bb4c6-129">5</span></span>|<span data-ttu-id="bb4c6-130">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="bb4c6-130">Release Windows Insider build</span></span>|




