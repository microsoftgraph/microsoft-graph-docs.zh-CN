---
title: windowsUpdateType 枚举类型
description: 将从哪些分支设备接收其更新
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e01f2e14e11558d79e0e5b420eac6fd0e359a813
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272330"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="dc91a-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dc91a-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="dc91a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc91a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc91a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dc91a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc91a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc91a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc91a-107">将从哪些分支设备接收其更新</span><span class="sxs-lookup"><span data-stu-id="dc91a-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="dc91a-108">成员</span><span class="sxs-lookup"><span data-stu-id="dc91a-108">Members</span></span>
|<span data-ttu-id="dc91a-109">成员</span><span class="sxs-lookup"><span data-stu-id="dc91a-109">Member</span></span>|<span data-ttu-id="dc91a-110">值</span><span class="sxs-lookup"><span data-stu-id="dc91a-110">Value</span></span>|<span data-ttu-id="dc91a-111">说明</span><span class="sxs-lookup"><span data-stu-id="dc91a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc91a-112">定制</span><span class="sxs-lookup"><span data-stu-id="dc91a-112">userDefined</span></span>|<span data-ttu-id="dc91a-113">0</span><span class="sxs-lookup"><span data-stu-id="dc91a-113">0</span></span>|<span data-ttu-id="dc91a-114">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="dc91a-114">Allow the user to set.</span></span>|
|<span data-ttu-id="dc91a-115">各种</span><span class="sxs-lookup"><span data-stu-id="dc91a-115">all</span></span>|<span data-ttu-id="dc91a-116">1</span><span class="sxs-lookup"><span data-stu-id="dc91a-116">1</span></span>|<span data-ttu-id="dc91a-117">目标) 的半年频道 (。</span><span class="sxs-lookup"><span data-stu-id="dc91a-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="dc91a-118">设备将从半年频道 (目标) 获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="dc91a-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="dc91a-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="dc91a-119">businessReadyOnly</span></span>|<span data-ttu-id="dc91a-120">双面</span><span class="sxs-lookup"><span data-stu-id="dc91a-120">2</span></span>|<span data-ttu-id="dc91a-121">半年频道。</span><span class="sxs-lookup"><span data-stu-id="dc91a-121">Semi-annual Channel.</span></span> <span data-ttu-id="dc91a-122">设备从半年频道获取功能更新。</span><span class="sxs-lookup"><span data-stu-id="dc91a-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="dc91a-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="dc91a-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="dc91a-124">第三章</span><span class="sxs-lookup"><span data-stu-id="dc91a-124">3</span></span>|<span data-ttu-id="dc91a-125">Windows 预览体验成员内部版本-快速</span><span class="sxs-lookup"><span data-stu-id="dc91a-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="dc91a-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="dc91a-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="dc91a-127">4 </span><span class="sxs-lookup"><span data-stu-id="dc91a-127">4</span></span>|<span data-ttu-id="dc91a-128">Windows 预览体验成员内部版本-慢</span><span class="sxs-lookup"><span data-stu-id="dc91a-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="dc91a-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="dc91a-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="dc91a-130">5 </span><span class="sxs-lookup"><span data-stu-id="dc91a-130">5</span></span>|<span data-ttu-id="dc91a-131">发布 Windows 预览体验成员内部版本</span><span class="sxs-lookup"><span data-stu-id="dc91a-131">Release Windows Insider build</span></span>|




