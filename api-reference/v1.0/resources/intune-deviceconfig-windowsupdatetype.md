---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: df2fb50d31720e1f919c23020dd739e1c604fd70
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532232"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="89192-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="89192-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="89192-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89192-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89192-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89192-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89192-106">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="89192-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="89192-107">成员</span><span class="sxs-lookup"><span data-stu-id="89192-107">Members</span></span>
|<span data-ttu-id="89192-108">成员</span><span class="sxs-lookup"><span data-stu-id="89192-108">Member</span></span>|<span data-ttu-id="89192-109">值</span><span class="sxs-lookup"><span data-stu-id="89192-109">Value</span></span>|<span data-ttu-id="89192-110">说明</span><span class="sxs-lookup"><span data-stu-id="89192-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89192-111">定制</span><span class="sxs-lookup"><span data-stu-id="89192-111">userDefined</span></span>|<span data-ttu-id="89192-112">0</span><span class="sxs-lookup"><span data-stu-id="89192-112">0</span></span>|<span data-ttu-id="89192-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="89192-113">Allow the user to set.</span></span>|
|<span data-ttu-id="89192-114">各种</span><span class="sxs-lookup"><span data-stu-id="89192-114">all</span></span>|<span data-ttu-id="89192-115">1 </span><span class="sxs-lookup"><span data-stu-id="89192-115">1</span></span>|<span data-ttu-id="89192-116">半年频道（定向）。</span><span class="sxs-lookup"><span data-stu-id="89192-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="89192-117">设备从半年频道（定向）获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="89192-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="89192-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="89192-118">businessReadyOnly</span></span>|<span data-ttu-id="89192-119">2 </span><span class="sxs-lookup"><span data-stu-id="89192-119">2</span></span>|<span data-ttu-id="89192-120">半年频道。</span><span class="sxs-lookup"><span data-stu-id="89192-120">Semi-annual Channel.</span></span> <span data-ttu-id="89192-121">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="89192-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="89192-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="89192-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="89192-123">3 </span><span class="sxs-lookup"><span data-stu-id="89192-123">3</span></span>|<span data-ttu-id="89192-124">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="89192-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="89192-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="89192-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="89192-126">4 </span><span class="sxs-lookup"><span data-stu-id="89192-126">4</span></span>|<span data-ttu-id="89192-127">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="89192-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="89192-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="89192-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="89192-129">5 </span><span class="sxs-lookup"><span data-stu-id="89192-129">5</span></span>|<span data-ttu-id="89192-130">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="89192-130">Release Windows Insider build</span></span>|




