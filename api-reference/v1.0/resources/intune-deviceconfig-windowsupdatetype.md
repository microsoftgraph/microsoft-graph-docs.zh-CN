---
title: windowsUpdateType 枚举类型
description: 分支的设备将接收从其更新
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90d1f946dd497e650df5eb07004560dda028e14f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930339"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="f690a-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f690a-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="f690a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f690a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f690a-105">分支的设备将接收从其更新</span><span class="sxs-lookup"><span data-stu-id="f690a-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="f690a-106">成员</span><span class="sxs-lookup"><span data-stu-id="f690a-106">Members</span></span>
|<span data-ttu-id="f690a-107">成员</span><span class="sxs-lookup"><span data-stu-id="f690a-107">Member</span></span>|<span data-ttu-id="f690a-108">值</span><span class="sxs-lookup"><span data-stu-id="f690a-108">Value</span></span>|<span data-ttu-id="f690a-109">Description</span><span class="sxs-lookup"><span data-stu-id="f690a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f690a-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="f690a-110">userDefined</span></span>|<span data-ttu-id="f690a-111">0</span><span class="sxs-lookup"><span data-stu-id="f690a-111">0</span></span>|<span data-ttu-id="f690a-112">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="f690a-112">Allow the user to set.</span></span>|
|<span data-ttu-id="f690a-113">all</span><span class="sxs-lookup"><span data-stu-id="f690a-113">all</span></span>|<span data-ttu-id="f690a-114">1</span><span class="sxs-lookup"><span data-stu-id="f690a-114">1</span></span>|<span data-ttu-id="f690a-115">半年 （目标） 通道。</span><span class="sxs-lookup"><span data-stu-id="f690a-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="f690a-116">设备从半年通道 （目标） 中获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="f690a-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="f690a-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="f690a-117">businessReadyOnly</span></span>|<span data-ttu-id="f690a-118">2</span><span class="sxs-lookup"><span data-stu-id="f690a-118">2</span></span>|<span data-ttu-id="f690a-119">半年通道。</span><span class="sxs-lookup"><span data-stu-id="f690a-119">Semi-annual Channel.</span></span> <span data-ttu-id="f690a-120">设备获取更新功能从半年通道。</span><span class="sxs-lookup"><span data-stu-id="f690a-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="f690a-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="f690a-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="f690a-122">3</span><span class="sxs-lookup"><span data-stu-id="f690a-122">3</span></span>|<span data-ttu-id="f690a-123">Windows 内幕生成-Fast</span><span class="sxs-lookup"><span data-stu-id="f690a-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="f690a-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="f690a-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="f690a-125">4</span><span class="sxs-lookup"><span data-stu-id="f690a-125">4</span></span>|<span data-ttu-id="f690a-126">Windows 内幕生成-速度较慢</span><span class="sxs-lookup"><span data-stu-id="f690a-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="f690a-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="f690a-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="f690a-128">5</span><span class="sxs-lookup"><span data-stu-id="f690a-128">5</span></span>|<span data-ttu-id="f690a-129">Windows 内幕发布版本</span><span class="sxs-lookup"><span data-stu-id="f690a-129">Release Windows Insider build</span></span>|



