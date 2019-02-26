---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f91657cabec59cf1307253d707ba632bf4f99463
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260219"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="7a5c0-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7a5c0-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="7a5c0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a5c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a5c0-105">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="7a5c0-105">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="7a5c0-106">成员</span><span class="sxs-lookup"><span data-stu-id="7a5c0-106">Members</span></span>
|<span data-ttu-id="7a5c0-107">成员</span><span class="sxs-lookup"><span data-stu-id="7a5c0-107">Member</span></span>|<span data-ttu-id="7a5c0-108">值</span><span class="sxs-lookup"><span data-stu-id="7a5c0-108">Value</span></span>|<span data-ttu-id="7a5c0-109">说明</span><span class="sxs-lookup"><span data-stu-id="7a5c0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a5c0-110">定制</span><span class="sxs-lookup"><span data-stu-id="7a5c0-110">userDefined</span></span>|<span data-ttu-id="7a5c0-111">0</span><span class="sxs-lookup"><span data-stu-id="7a5c0-111">0</span></span>|<span data-ttu-id="7a5c0-112">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="7a5c0-112">Allow the user to set.</span></span>|
|<span data-ttu-id="7a5c0-113">all</span><span class="sxs-lookup"><span data-stu-id="7a5c0-113">all</span></span>|<span data-ttu-id="7a5c0-114">1</span><span class="sxs-lookup"><span data-stu-id="7a5c0-114">1</span></span>|<span data-ttu-id="7a5c0-115">半年频道 (定向)。</span><span class="sxs-lookup"><span data-stu-id="7a5c0-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="7a5c0-116">设备从半年频道 (定向) 获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="7a5c0-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="7a5c0-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="7a5c0-117">businessReadyOnly</span></span>|<span data-ttu-id="7a5c0-118">双面</span><span class="sxs-lookup"><span data-stu-id="7a5c0-118">2</span></span>|<span data-ttu-id="7a5c0-119">半年频道。</span><span class="sxs-lookup"><span data-stu-id="7a5c0-119">Semi-annual Channel.</span></span> <span data-ttu-id="7a5c0-120">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="7a5c0-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="7a5c0-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="7a5c0-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="7a5c0-122">第三章</span><span class="sxs-lookup"><span data-stu-id="7a5c0-122">3</span></span>|<span data-ttu-id="7a5c0-123">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="7a5c0-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="7a5c0-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="7a5c0-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="7a5c0-125">4</span><span class="sxs-lookup"><span data-stu-id="7a5c0-125">4</span></span>|<span data-ttu-id="7a5c0-126">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="7a5c0-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="7a5c0-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="7a5c0-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="7a5c0-128">5</span><span class="sxs-lookup"><span data-stu-id="7a5c0-128">5</span></span>|<span data-ttu-id="7a5c0-129">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="7a5c0-129">Release Windows Insider build</span></span>|



