---
title: windowsUpdateType 枚举类型
description: 分支的设备将接收从其更新
ms.openlocfilehash: b489f17da5dc02dd7f7e72350eef282e56643dd0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011292"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="b66f2-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b66f2-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="b66f2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b66f2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b66f2-105">分支的设备将接收从其更新</span><span class="sxs-lookup"><span data-stu-id="b66f2-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="b66f2-106">成员</span><span class="sxs-lookup"><span data-stu-id="b66f2-106">Members</span></span>
|<span data-ttu-id="b66f2-107">成员</span><span class="sxs-lookup"><span data-stu-id="b66f2-107">Member</span></span>|<span data-ttu-id="b66f2-108">值</span><span class="sxs-lookup"><span data-stu-id="b66f2-108">Value</span></span>|<span data-ttu-id="b66f2-109">说明</span><span class="sxs-lookup"><span data-stu-id="b66f2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b66f2-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="b66f2-110">userDefined</span></span>|<span data-ttu-id="b66f2-111">0</span><span class="sxs-lookup"><span data-stu-id="b66f2-111">0</span></span>|<span data-ttu-id="b66f2-112">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="b66f2-112">Allow the user to set.</span></span>|
|<span data-ttu-id="b66f2-113">all</span><span class="sxs-lookup"><span data-stu-id="b66f2-113">all</span></span>|<span data-ttu-id="b66f2-114">1</span><span class="sxs-lookup"><span data-stu-id="b66f2-114">1</span></span>|<span data-ttu-id="b66f2-115">半年 （目标） 通道。</span><span class="sxs-lookup"><span data-stu-id="b66f2-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="b66f2-116">设备从半年通道 （目标） 中获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="b66f2-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="b66f2-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="b66f2-117">businessReadyOnly</span></span>|<span data-ttu-id="b66f2-118">2</span><span class="sxs-lookup"><span data-stu-id="b66f2-118">2</span></span>|<span data-ttu-id="b66f2-119">半年通道。</span><span class="sxs-lookup"><span data-stu-id="b66f2-119">Semi-annual Channel.</span></span> <span data-ttu-id="b66f2-120">设备获取更新功能从半年通道。</span><span class="sxs-lookup"><span data-stu-id="b66f2-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="b66f2-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="b66f2-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="b66f2-122">3</span><span class="sxs-lookup"><span data-stu-id="b66f2-122">3</span></span>|<span data-ttu-id="b66f2-123">Windows 内幕生成-Fast</span><span class="sxs-lookup"><span data-stu-id="b66f2-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="b66f2-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="b66f2-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="b66f2-125">4</span><span class="sxs-lookup"><span data-stu-id="b66f2-125">4</span></span>|<span data-ttu-id="b66f2-126">Windows 内幕生成-速度较慢</span><span class="sxs-lookup"><span data-stu-id="b66f2-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="b66f2-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="b66f2-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="b66f2-128">5</span><span class="sxs-lookup"><span data-stu-id="b66f2-128">5</span></span>|<span data-ttu-id="b66f2-129">Windows 内幕发布版本</span><span class="sxs-lookup"><span data-stu-id="b66f2-129">Release Windows Insider build</span></span>|



