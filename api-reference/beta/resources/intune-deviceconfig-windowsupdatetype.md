---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 35fe62ada736a0cd5c3a073e49851b6cad9320ab
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786149"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="33213-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="33213-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="33213-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="33213-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33213-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="33213-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33213-106">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="33213-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="33213-107">成员</span><span class="sxs-lookup"><span data-stu-id="33213-107">Members</span></span>
|<span data-ttu-id="33213-108">成员</span><span class="sxs-lookup"><span data-stu-id="33213-108">Member</span></span>|<span data-ttu-id="33213-109">值</span><span class="sxs-lookup"><span data-stu-id="33213-109">Value</span></span>|<span data-ttu-id="33213-110">说明</span><span class="sxs-lookup"><span data-stu-id="33213-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33213-111">定制</span><span class="sxs-lookup"><span data-stu-id="33213-111">userDefined</span></span>|<span data-ttu-id="33213-112">0</span><span class="sxs-lookup"><span data-stu-id="33213-112">0</span></span>|<span data-ttu-id="33213-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="33213-113">Allow the user to set.</span></span>|
|<span data-ttu-id="33213-114">各种</span><span class="sxs-lookup"><span data-stu-id="33213-114">all</span></span>|<span data-ttu-id="33213-115">1</span><span class="sxs-lookup"><span data-stu-id="33213-115">1</span></span>|<span data-ttu-id="33213-116">半年频道（定向）。</span><span class="sxs-lookup"><span data-stu-id="33213-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="33213-117">设备从半年频道（定向）获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="33213-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="33213-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="33213-118">businessReadyOnly</span></span>|<span data-ttu-id="33213-119">双面</span><span class="sxs-lookup"><span data-stu-id="33213-119">2</span></span>|<span data-ttu-id="33213-120">半年频道。</span><span class="sxs-lookup"><span data-stu-id="33213-120">Semi-annual Channel.</span></span> <span data-ttu-id="33213-121">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="33213-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="33213-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="33213-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="33213-123">第三章</span><span class="sxs-lookup"><span data-stu-id="33213-123">3</span></span>|<span data-ttu-id="33213-124">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="33213-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="33213-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="33213-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="33213-126">4 </span><span class="sxs-lookup"><span data-stu-id="33213-126">4</span></span>|<span data-ttu-id="33213-127">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="33213-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="33213-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="33213-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="33213-129">5 </span><span class="sxs-lookup"><span data-stu-id="33213-129">5</span></span>|<span data-ttu-id="33213-130">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="33213-130">Release Windows Insider build</span></span>|



