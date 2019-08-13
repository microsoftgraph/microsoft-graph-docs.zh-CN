---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 41a6d23e42d263dd8241e960af693450ac0a7c3d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369505"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="e7d57-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e7d57-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="e7d57-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7d57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7d57-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7d57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7d57-106">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="e7d57-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="e7d57-107">成员</span><span class="sxs-lookup"><span data-stu-id="e7d57-107">Members</span></span>
|<span data-ttu-id="e7d57-108">成员</span><span class="sxs-lookup"><span data-stu-id="e7d57-108">Member</span></span>|<span data-ttu-id="e7d57-109">值</span><span class="sxs-lookup"><span data-stu-id="e7d57-109">Value</span></span>|<span data-ttu-id="e7d57-110">说明</span><span class="sxs-lookup"><span data-stu-id="e7d57-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7d57-111">定制</span><span class="sxs-lookup"><span data-stu-id="e7d57-111">userDefined</span></span>|<span data-ttu-id="e7d57-112">0</span><span class="sxs-lookup"><span data-stu-id="e7d57-112">0</span></span>|<span data-ttu-id="e7d57-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="e7d57-113">Allow the user to set.</span></span>|
|<span data-ttu-id="e7d57-114">各种</span><span class="sxs-lookup"><span data-stu-id="e7d57-114">all</span></span>|<span data-ttu-id="e7d57-115">1</span><span class="sxs-lookup"><span data-stu-id="e7d57-115">1</span></span>|<span data-ttu-id="e7d57-116">半年频道 (定向)。</span><span class="sxs-lookup"><span data-stu-id="e7d57-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="e7d57-117">设备从半年频道 (定向) 获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="e7d57-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="e7d57-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="e7d57-118">businessReadyOnly</span></span>|<span data-ttu-id="e7d57-119">双面</span><span class="sxs-lookup"><span data-stu-id="e7d57-119">2</span></span>|<span data-ttu-id="e7d57-120">半年频道。</span><span class="sxs-lookup"><span data-stu-id="e7d57-120">Semi-annual Channel.</span></span> <span data-ttu-id="e7d57-121">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="e7d57-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="e7d57-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="e7d57-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="e7d57-123">第三章</span><span class="sxs-lookup"><span data-stu-id="e7d57-123">3</span></span>|<span data-ttu-id="e7d57-124">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="e7d57-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="e7d57-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="e7d57-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="e7d57-126">4</span><span class="sxs-lookup"><span data-stu-id="e7d57-126">4</span></span>|<span data-ttu-id="e7d57-127">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="e7d57-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="e7d57-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="e7d57-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="e7d57-129">5</span><span class="sxs-lookup"><span data-stu-id="e7d57-129">5</span></span>|<span data-ttu-id="e7d57-130">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="e7d57-130">Release Windows Insider build</span></span>|



