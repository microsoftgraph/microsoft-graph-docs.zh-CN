---
title: windowsUpdateType 枚举类型
description: 哪些分支设备将接收其更新
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f49158686884d55825751a9314a50a9ab9a16d57
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759943"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="03a93-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="03a93-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="03a93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03a93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03a93-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03a93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03a93-106">哪些分支设备将接收其更新</span><span class="sxs-lookup"><span data-stu-id="03a93-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="03a93-107">成员</span><span class="sxs-lookup"><span data-stu-id="03a93-107">Members</span></span>
|<span data-ttu-id="03a93-108">成员</span><span class="sxs-lookup"><span data-stu-id="03a93-108">Member</span></span>|<span data-ttu-id="03a93-109">值</span><span class="sxs-lookup"><span data-stu-id="03a93-109">Value</span></span>|<span data-ttu-id="03a93-110">说明</span><span class="sxs-lookup"><span data-stu-id="03a93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03a93-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="03a93-111">userDefined</span></span>|<span data-ttu-id="03a93-112">0</span><span class="sxs-lookup"><span data-stu-id="03a93-112">0</span></span>|<span data-ttu-id="03a93-113">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="03a93-113">Allow the user to set.</span></span>|
|<span data-ttu-id="03a93-114">all</span><span class="sxs-lookup"><span data-stu-id="03a93-114">all</span></span>|<span data-ttu-id="03a93-115">1</span><span class="sxs-lookup"><span data-stu-id="03a93-115">1</span></span>|<span data-ttu-id="03a93-116">半年频道 (定向) 。</span><span class="sxs-lookup"><span data-stu-id="03a93-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="03a93-117">设备从半年频道和目标用户获取 (功能) 。</span><span class="sxs-lookup"><span data-stu-id="03a93-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="03a93-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="03a93-118">businessReadyOnly</span></span>|<span data-ttu-id="03a93-119">2</span><span class="sxs-lookup"><span data-stu-id="03a93-119">2</span></span>|<span data-ttu-id="03a93-120">半年频道。</span><span class="sxs-lookup"><span data-stu-id="03a93-120">Semi-annual Channel.</span></span> <span data-ttu-id="03a93-121">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="03a93-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="03a93-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="03a93-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="03a93-123">3</span><span class="sxs-lookup"><span data-stu-id="03a93-123">3</span></span>|<span data-ttu-id="03a93-124">Windows预览体验成员内部版本 - 快速</span><span class="sxs-lookup"><span data-stu-id="03a93-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="03a93-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="03a93-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="03a93-126">4 </span><span class="sxs-lookup"><span data-stu-id="03a93-126">4</span></span>|<span data-ttu-id="03a93-127">Windows预览体验成员内部版本 - 慢</span><span class="sxs-lookup"><span data-stu-id="03a93-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="03a93-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="03a93-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="03a93-129">5 </span><span class="sxs-lookup"><span data-stu-id="03a93-129">5</span></span>|<span data-ttu-id="03a93-130">预览Windows内部版本</span><span class="sxs-lookup"><span data-stu-id="03a93-130">Release Windows Insider build</span></span>|




