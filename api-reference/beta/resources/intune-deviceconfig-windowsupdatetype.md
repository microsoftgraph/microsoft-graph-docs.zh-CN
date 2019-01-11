---
title: windowsUpdateType 枚举类型
description: 分支的设备将接收从其更新
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 15d2d46684d38b57690cc9c12d9c49eccd652e6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887036"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="88bc6-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="88bc6-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="88bc6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="88bc6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88bc6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88bc6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88bc6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="88bc6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88bc6-107">分支的设备将接收从其更新</span><span class="sxs-lookup"><span data-stu-id="88bc6-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="88bc6-108">成员</span><span class="sxs-lookup"><span data-stu-id="88bc6-108">Members</span></span>
|<span data-ttu-id="88bc6-109">成员</span><span class="sxs-lookup"><span data-stu-id="88bc6-109">Member</span></span>|<span data-ttu-id="88bc6-110">值</span><span class="sxs-lookup"><span data-stu-id="88bc6-110">Value</span></span>|<span data-ttu-id="88bc6-111">Description</span><span class="sxs-lookup"><span data-stu-id="88bc6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88bc6-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="88bc6-112">userDefined</span></span>|<span data-ttu-id="88bc6-113">0</span><span class="sxs-lookup"><span data-stu-id="88bc6-113">0</span></span>|<span data-ttu-id="88bc6-114">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="88bc6-114">Allow the user to set.</span></span>|
|<span data-ttu-id="88bc6-115">all</span><span class="sxs-lookup"><span data-stu-id="88bc6-115">all</span></span>|<span data-ttu-id="88bc6-116">1</span><span class="sxs-lookup"><span data-stu-id="88bc6-116">1</span></span>|<span data-ttu-id="88bc6-117">半年 （目标） 通道。</span><span class="sxs-lookup"><span data-stu-id="88bc6-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="88bc6-118">设备从半年通道 （目标） 中获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="88bc6-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="88bc6-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="88bc6-119">businessReadyOnly</span></span>|<span data-ttu-id="88bc6-120">2</span><span class="sxs-lookup"><span data-stu-id="88bc6-120">2</span></span>|<span data-ttu-id="88bc6-121">半年通道。</span><span class="sxs-lookup"><span data-stu-id="88bc6-121">Semi-annual Channel.</span></span> <span data-ttu-id="88bc6-122">设备获取更新功能从半年通道。</span><span class="sxs-lookup"><span data-stu-id="88bc6-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="88bc6-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="88bc6-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="88bc6-124">3</span><span class="sxs-lookup"><span data-stu-id="88bc6-124">3</span></span>|<span data-ttu-id="88bc6-125">Windows 内幕生成-Fast</span><span class="sxs-lookup"><span data-stu-id="88bc6-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="88bc6-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="88bc6-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="88bc6-127">4</span><span class="sxs-lookup"><span data-stu-id="88bc6-127">4</span></span>|<span data-ttu-id="88bc6-128">Windows 内幕生成-速度较慢</span><span class="sxs-lookup"><span data-stu-id="88bc6-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="88bc6-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="88bc6-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="88bc6-130">5</span><span class="sxs-lookup"><span data-stu-id="88bc6-130">5</span></span>|<span data-ttu-id="88bc6-131">Windows 内幕发布版本</span><span class="sxs-lookup"><span data-stu-id="88bc6-131">Release Windows Insider build</span></span>|





