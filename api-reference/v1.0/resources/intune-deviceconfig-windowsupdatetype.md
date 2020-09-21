---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b139112db8a106dfa57c7d3ddb98e2415294914b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091374"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="12a67-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="12a67-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="12a67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12a67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12a67-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12a67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12a67-106">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="12a67-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="12a67-107">成员</span><span class="sxs-lookup"><span data-stu-id="12a67-107">Members</span></span>
|<span data-ttu-id="12a67-108">成员</span><span class="sxs-lookup"><span data-stu-id="12a67-108">Member</span></span>|<span data-ttu-id="12a67-109">值</span><span class="sxs-lookup"><span data-stu-id="12a67-109">Value</span></span>|<span data-ttu-id="12a67-110">说明</span><span class="sxs-lookup"><span data-stu-id="12a67-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12a67-111">定制</span><span class="sxs-lookup"><span data-stu-id="12a67-111">userDefined</span></span>|<span data-ttu-id="12a67-112">0</span><span class="sxs-lookup"><span data-stu-id="12a67-112">0</span></span>|<span data-ttu-id="12a67-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="12a67-113">Allow the user to set.</span></span>|
|<span data-ttu-id="12a67-114">各种</span><span class="sxs-lookup"><span data-stu-id="12a67-114">all</span></span>|<span data-ttu-id="12a67-115">1 </span><span class="sxs-lookup"><span data-stu-id="12a67-115">1</span></span>|<span data-ttu-id="12a67-116">目标) 的半年频道 (。</span><span class="sxs-lookup"><span data-stu-id="12a67-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="12a67-117">设备将从半年频道 (目标) 获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="12a67-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="12a67-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="12a67-118">businessReadyOnly</span></span>|<span data-ttu-id="12a67-119">2 </span><span class="sxs-lookup"><span data-stu-id="12a67-119">2</span></span>|<span data-ttu-id="12a67-120">半年频道。</span><span class="sxs-lookup"><span data-stu-id="12a67-120">Semi-annual Channel.</span></span> <span data-ttu-id="12a67-121">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="12a67-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="12a67-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="12a67-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="12a67-123">第三章</span><span class="sxs-lookup"><span data-stu-id="12a67-123">3</span></span>|<span data-ttu-id="12a67-124">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="12a67-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="12a67-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="12a67-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="12a67-126">4 </span><span class="sxs-lookup"><span data-stu-id="12a67-126">4</span></span>|<span data-ttu-id="12a67-127">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="12a67-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="12a67-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="12a67-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="12a67-129">5 </span><span class="sxs-lookup"><span data-stu-id="12a67-129">5</span></span>|<span data-ttu-id="12a67-130">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="12a67-130">Release Windows Insider build</span></span>|









