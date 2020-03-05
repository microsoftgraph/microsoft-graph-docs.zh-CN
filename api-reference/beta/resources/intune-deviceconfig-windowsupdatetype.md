---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 94c82e45aae328f35b890f82755609945a9b58f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528930"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="ebd58-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ebd58-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="ebd58-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ebd58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebd58-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ebd58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebd58-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebd58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebd58-107">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="ebd58-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="ebd58-108">成员</span><span class="sxs-lookup"><span data-stu-id="ebd58-108">Members</span></span>
|<span data-ttu-id="ebd58-109">成员</span><span class="sxs-lookup"><span data-stu-id="ebd58-109">Member</span></span>|<span data-ttu-id="ebd58-110">值</span><span class="sxs-lookup"><span data-stu-id="ebd58-110">Value</span></span>|<span data-ttu-id="ebd58-111">说明</span><span class="sxs-lookup"><span data-stu-id="ebd58-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebd58-112">定制</span><span class="sxs-lookup"><span data-stu-id="ebd58-112">userDefined</span></span>|<span data-ttu-id="ebd58-113">0</span><span class="sxs-lookup"><span data-stu-id="ebd58-113">0</span></span>|<span data-ttu-id="ebd58-114">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="ebd58-114">Allow the user to set.</span></span>|
|<span data-ttu-id="ebd58-115">各种</span><span class="sxs-lookup"><span data-stu-id="ebd58-115">all</span></span>|<span data-ttu-id="ebd58-116">1 </span><span class="sxs-lookup"><span data-stu-id="ebd58-116">1</span></span>|<span data-ttu-id="ebd58-117">半年频道（定向）。</span><span class="sxs-lookup"><span data-stu-id="ebd58-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="ebd58-118">设备从半年频道（定向）获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="ebd58-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="ebd58-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="ebd58-119">businessReadyOnly</span></span>|<span data-ttu-id="ebd58-120">2 </span><span class="sxs-lookup"><span data-stu-id="ebd58-120">2</span></span>|<span data-ttu-id="ebd58-121">半年频道。</span><span class="sxs-lookup"><span data-stu-id="ebd58-121">Semi-annual Channel.</span></span> <span data-ttu-id="ebd58-122">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="ebd58-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="ebd58-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="ebd58-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="ebd58-124">3 </span><span class="sxs-lookup"><span data-stu-id="ebd58-124">3</span></span>|<span data-ttu-id="ebd58-125">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="ebd58-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="ebd58-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="ebd58-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="ebd58-127">4 </span><span class="sxs-lookup"><span data-stu-id="ebd58-127">4</span></span>|<span data-ttu-id="ebd58-128">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="ebd58-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="ebd58-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="ebd58-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="ebd58-130">5 </span><span class="sxs-lookup"><span data-stu-id="ebd58-130">5</span></span>|<span data-ttu-id="ebd58-131">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="ebd58-131">Release Windows Insider build</span></span>|



