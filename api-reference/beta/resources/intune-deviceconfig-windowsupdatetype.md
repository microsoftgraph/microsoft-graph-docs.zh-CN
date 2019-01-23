---
title: windowsUpdateType 枚举类型
description: 分支的设备将接收从其更新
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d3dd0f6d8ba46d7f1cc803b217a98a862602149
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400135"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="6d9b8-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6d9b8-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="6d9b8-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6d9b8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6d9b8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6d9b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d9b8-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d9b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d9b8-107">分支的设备将接收从其更新</span><span class="sxs-lookup"><span data-stu-id="6d9b8-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="6d9b8-108">成员</span><span class="sxs-lookup"><span data-stu-id="6d9b8-108">Members</span></span>
|<span data-ttu-id="6d9b8-109">成员</span><span class="sxs-lookup"><span data-stu-id="6d9b8-109">Member</span></span>|<span data-ttu-id="6d9b8-110">值</span><span class="sxs-lookup"><span data-stu-id="6d9b8-110">Value</span></span>|<span data-ttu-id="6d9b8-111">说明</span><span class="sxs-lookup"><span data-stu-id="6d9b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d9b8-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="6d9b8-112">userDefined</span></span>|<span data-ttu-id="6d9b8-113">0</span><span class="sxs-lookup"><span data-stu-id="6d9b8-113">0</span></span>|<span data-ttu-id="6d9b8-114">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="6d9b8-114">Allow the user to set.</span></span>|
|<span data-ttu-id="6d9b8-115">all</span><span class="sxs-lookup"><span data-stu-id="6d9b8-115">all</span></span>|<span data-ttu-id="6d9b8-116">1</span><span class="sxs-lookup"><span data-stu-id="6d9b8-116">1</span></span>|<span data-ttu-id="6d9b8-117">半年 （目标） 通道。</span><span class="sxs-lookup"><span data-stu-id="6d9b8-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="6d9b8-118">设备从半年通道 （目标） 中获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="6d9b8-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="6d9b8-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="6d9b8-119">businessReadyOnly</span></span>|<span data-ttu-id="6d9b8-120">2</span><span class="sxs-lookup"><span data-stu-id="6d9b8-120">2</span></span>|<span data-ttu-id="6d9b8-121">半年通道。</span><span class="sxs-lookup"><span data-stu-id="6d9b8-121">Semi-annual Channel.</span></span> <span data-ttu-id="6d9b8-122">设备获取更新功能从半年通道。</span><span class="sxs-lookup"><span data-stu-id="6d9b8-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="6d9b8-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="6d9b8-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="6d9b8-124">3</span><span class="sxs-lookup"><span data-stu-id="6d9b8-124">3</span></span>|<span data-ttu-id="6d9b8-125">Windows 内幕生成-Fast</span><span class="sxs-lookup"><span data-stu-id="6d9b8-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="6d9b8-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="6d9b8-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="6d9b8-127">4</span><span class="sxs-lookup"><span data-stu-id="6d9b8-127">4</span></span>|<span data-ttu-id="6d9b8-128">Windows 内幕生成-速度较慢</span><span class="sxs-lookup"><span data-stu-id="6d9b8-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="6d9b8-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="6d9b8-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="6d9b8-130">5</span><span class="sxs-lookup"><span data-stu-id="6d9b8-130">5</span></span>|<span data-ttu-id="6d9b8-131">Windows 内幕发布版本</span><span class="sxs-lookup"><span data-stu-id="6d9b8-131">Release Windows Insider build</span></span>|




