---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 228cc5ba4b50681bfe78a15ef214d6f3ab2ebb17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523593"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="55d16-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="55d16-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="55d16-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="55d16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55d16-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55d16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55d16-106">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="55d16-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="55d16-107">成员</span><span class="sxs-lookup"><span data-stu-id="55d16-107">Members</span></span>
|<span data-ttu-id="55d16-108">成员</span><span class="sxs-lookup"><span data-stu-id="55d16-108">Member</span></span>|<span data-ttu-id="55d16-109">值</span><span class="sxs-lookup"><span data-stu-id="55d16-109">Value</span></span>|<span data-ttu-id="55d16-110">说明</span><span class="sxs-lookup"><span data-stu-id="55d16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55d16-111">定制</span><span class="sxs-lookup"><span data-stu-id="55d16-111">userDefined</span></span>|<span data-ttu-id="55d16-112">0</span><span class="sxs-lookup"><span data-stu-id="55d16-112">0</span></span>|<span data-ttu-id="55d16-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="55d16-113">Allow the user to set.</span></span>|
|<span data-ttu-id="55d16-114">各种</span><span class="sxs-lookup"><span data-stu-id="55d16-114">all</span></span>|<span data-ttu-id="55d16-115">1</span><span class="sxs-lookup"><span data-stu-id="55d16-115">1</span></span>|<span data-ttu-id="55d16-116">半年频道 (定向)。</span><span class="sxs-lookup"><span data-stu-id="55d16-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="55d16-117">设备从半年频道 (定向) 获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="55d16-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="55d16-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="55d16-118">businessReadyOnly</span></span>|<span data-ttu-id="55d16-119">2 </span><span class="sxs-lookup"><span data-stu-id="55d16-119">2</span></span>|<span data-ttu-id="55d16-120">半年频道。</span><span class="sxs-lookup"><span data-stu-id="55d16-120">Semi-annual Channel.</span></span> <span data-ttu-id="55d16-121">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="55d16-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="55d16-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="55d16-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="55d16-123">3 </span><span class="sxs-lookup"><span data-stu-id="55d16-123">3</span></span>|<span data-ttu-id="55d16-124">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="55d16-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="55d16-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="55d16-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="55d16-126">4 </span><span class="sxs-lookup"><span data-stu-id="55d16-126">4</span></span>|<span data-ttu-id="55d16-127">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="55d16-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="55d16-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="55d16-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="55d16-129">5 </span><span class="sxs-lookup"><span data-stu-id="55d16-129">5</span></span>|<span data-ttu-id="55d16-130">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="55d16-130">Release Windows Insider build</span></span>|





