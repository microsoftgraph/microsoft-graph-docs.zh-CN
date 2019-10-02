---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e0868516f84d15ff18a3b54c2ebfb936fb1641ed
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357127"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="33a6d-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="33a6d-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="33a6d-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="33a6d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33a6d-105">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="33a6d-105">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="33a6d-106">成员</span><span class="sxs-lookup"><span data-stu-id="33a6d-106">Members</span></span>
|<span data-ttu-id="33a6d-107">成员</span><span class="sxs-lookup"><span data-stu-id="33a6d-107">Member</span></span>|<span data-ttu-id="33a6d-108">值</span><span class="sxs-lookup"><span data-stu-id="33a6d-108">Value</span></span>|<span data-ttu-id="33a6d-109">说明</span><span class="sxs-lookup"><span data-stu-id="33a6d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33a6d-110">定制</span><span class="sxs-lookup"><span data-stu-id="33a6d-110">userDefined</span></span>|<span data-ttu-id="33a6d-111">0</span><span class="sxs-lookup"><span data-stu-id="33a6d-111">0</span></span>|<span data-ttu-id="33a6d-112">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="33a6d-112">Allow the user to set.</span></span>|
|<span data-ttu-id="33a6d-113">各种</span><span class="sxs-lookup"><span data-stu-id="33a6d-113">all</span></span>|<span data-ttu-id="33a6d-114">1</span><span class="sxs-lookup"><span data-stu-id="33a6d-114">1</span></span>|<span data-ttu-id="33a6d-115">半年频道（定向）。</span><span class="sxs-lookup"><span data-stu-id="33a6d-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="33a6d-116">设备从半年频道（定向）获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="33a6d-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="33a6d-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="33a6d-117">businessReadyOnly</span></span>|<span data-ttu-id="33a6d-118">双面</span><span class="sxs-lookup"><span data-stu-id="33a6d-118">2</span></span>|<span data-ttu-id="33a6d-119">半年频道。</span><span class="sxs-lookup"><span data-stu-id="33a6d-119">Semi-annual Channel.</span></span> <span data-ttu-id="33a6d-120">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="33a6d-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="33a6d-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="33a6d-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="33a6d-122">第三章</span><span class="sxs-lookup"><span data-stu-id="33a6d-122">3</span></span>|<span data-ttu-id="33a6d-123">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="33a6d-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="33a6d-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="33a6d-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="33a6d-125">4</span><span class="sxs-lookup"><span data-stu-id="33a6d-125">4</span></span>|<span data-ttu-id="33a6d-126">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="33a6d-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="33a6d-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="33a6d-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="33a6d-128">5</span><span class="sxs-lookup"><span data-stu-id="33a6d-128">5</span></span>|<span data-ttu-id="33a6d-129">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="33a6d-129">Release Windows Insider build</span></span>|




