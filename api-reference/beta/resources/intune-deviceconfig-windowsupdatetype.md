---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f971b39d1b9ef96d9163c0ac38d8505297c6754f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706924"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="07d8e-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="07d8e-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="07d8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07d8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07d8e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07d8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07d8e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07d8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07d8e-107">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="07d8e-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="07d8e-108">成员</span><span class="sxs-lookup"><span data-stu-id="07d8e-108">Members</span></span>
|<span data-ttu-id="07d8e-109">成员</span><span class="sxs-lookup"><span data-stu-id="07d8e-109">Member</span></span>|<span data-ttu-id="07d8e-110">值</span><span class="sxs-lookup"><span data-stu-id="07d8e-110">Value</span></span>|<span data-ttu-id="07d8e-111">说明</span><span class="sxs-lookup"><span data-stu-id="07d8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07d8e-112">定制</span><span class="sxs-lookup"><span data-stu-id="07d8e-112">userDefined</span></span>|<span data-ttu-id="07d8e-113">0</span><span class="sxs-lookup"><span data-stu-id="07d8e-113">0</span></span>|<span data-ttu-id="07d8e-114">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="07d8e-114">Allow the user to set.</span></span>|
|<span data-ttu-id="07d8e-115">各种</span><span class="sxs-lookup"><span data-stu-id="07d8e-115">all</span></span>|<span data-ttu-id="07d8e-116">1</span><span class="sxs-lookup"><span data-stu-id="07d8e-116">1</span></span>|<span data-ttu-id="07d8e-117">目标) 的半年频道 (。</span><span class="sxs-lookup"><span data-stu-id="07d8e-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="07d8e-118">设备将从半年频道 (目标) 获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="07d8e-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="07d8e-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="07d8e-119">businessReadyOnly</span></span>|<span data-ttu-id="07d8e-120">双面</span><span class="sxs-lookup"><span data-stu-id="07d8e-120">2</span></span>|<span data-ttu-id="07d8e-121">半年频道。</span><span class="sxs-lookup"><span data-stu-id="07d8e-121">Semi-annual Channel.</span></span> <span data-ttu-id="07d8e-122">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="07d8e-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="07d8e-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="07d8e-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="07d8e-124">第三章</span><span class="sxs-lookup"><span data-stu-id="07d8e-124">3</span></span>|<span data-ttu-id="07d8e-125">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="07d8e-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="07d8e-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="07d8e-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="07d8e-127">4 </span><span class="sxs-lookup"><span data-stu-id="07d8e-127">4</span></span>|<span data-ttu-id="07d8e-128">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="07d8e-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="07d8e-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="07d8e-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="07d8e-130">5 </span><span class="sxs-lookup"><span data-stu-id="07d8e-130">5</span></span>|<span data-ttu-id="07d8e-131">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="07d8e-131">Release Windows Insider build</span></span>|





