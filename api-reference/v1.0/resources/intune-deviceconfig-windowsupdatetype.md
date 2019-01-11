---
title: windowsUpdateType 枚举类型
description: 分支的设备将接收从其更新
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 198b5f8db5698d309199964e4cb69f8981ceeb1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838967"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="f836c-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f836c-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="f836c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f836c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f836c-105">分支的设备将接收从其更新</span><span class="sxs-lookup"><span data-stu-id="f836c-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="f836c-106">成员</span><span class="sxs-lookup"><span data-stu-id="f836c-106">Members</span></span>
|<span data-ttu-id="f836c-107">成员</span><span class="sxs-lookup"><span data-stu-id="f836c-107">Member</span></span>|<span data-ttu-id="f836c-108">值</span><span class="sxs-lookup"><span data-stu-id="f836c-108">Value</span></span>|<span data-ttu-id="f836c-109">Description</span><span class="sxs-lookup"><span data-stu-id="f836c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f836c-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="f836c-110">userDefined</span></span>|<span data-ttu-id="f836c-111">0</span><span class="sxs-lookup"><span data-stu-id="f836c-111">0</span></span>|<span data-ttu-id="f836c-112">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="f836c-112">Allow the user to set.</span></span>|
|<span data-ttu-id="f836c-113">all</span><span class="sxs-lookup"><span data-stu-id="f836c-113">all</span></span>|<span data-ttu-id="f836c-114">1</span><span class="sxs-lookup"><span data-stu-id="f836c-114">1</span></span>|<span data-ttu-id="f836c-115">半年 （目标） 通道。</span><span class="sxs-lookup"><span data-stu-id="f836c-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="f836c-116">设备从半年通道 （目标） 中获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="f836c-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="f836c-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="f836c-117">businessReadyOnly</span></span>|<span data-ttu-id="f836c-118">2</span><span class="sxs-lookup"><span data-stu-id="f836c-118">2</span></span>|<span data-ttu-id="f836c-119">半年通道。</span><span class="sxs-lookup"><span data-stu-id="f836c-119">Semi-annual Channel.</span></span> <span data-ttu-id="f836c-120">设备获取更新功能从半年通道。</span><span class="sxs-lookup"><span data-stu-id="f836c-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="f836c-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="f836c-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="f836c-122">3</span><span class="sxs-lookup"><span data-stu-id="f836c-122">3</span></span>|<span data-ttu-id="f836c-123">Windows 内幕生成-Fast</span><span class="sxs-lookup"><span data-stu-id="f836c-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="f836c-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="f836c-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="f836c-125">4</span><span class="sxs-lookup"><span data-stu-id="f836c-125">4</span></span>|<span data-ttu-id="f836c-126">Windows 内幕生成-速度较慢</span><span class="sxs-lookup"><span data-stu-id="f836c-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="f836c-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="f836c-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="f836c-128">5</span><span class="sxs-lookup"><span data-stu-id="f836c-128">5</span></span>|<span data-ttu-id="f836c-129">Windows 内幕发布版本</span><span class="sxs-lookup"><span data-stu-id="f836c-129">Release Windows Insider build</span></span>|



