---
title: windowsUpdateType 枚举类型
description: 分支的设备将接收从其更新
ms.openlocfilehash: 7669caa27be93786d381266f88b41ae456314bb4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049249"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="1d45d-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1d45d-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="1d45d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1d45d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d45d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1d45d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d45d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1d45d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d45d-107">分支的设备将接收从其更新</span><span class="sxs-lookup"><span data-stu-id="1d45d-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="1d45d-108">成员</span><span class="sxs-lookup"><span data-stu-id="1d45d-108">Members</span></span>
|<span data-ttu-id="1d45d-109">成员</span><span class="sxs-lookup"><span data-stu-id="1d45d-109">Member</span></span>|<span data-ttu-id="1d45d-110">值</span><span class="sxs-lookup"><span data-stu-id="1d45d-110">Value</span></span>|<span data-ttu-id="1d45d-111">说明</span><span class="sxs-lookup"><span data-stu-id="1d45d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d45d-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="1d45d-112">userDefined</span></span>|<span data-ttu-id="1d45d-113">0</span><span class="sxs-lookup"><span data-stu-id="1d45d-113">0</span></span>|<span data-ttu-id="1d45d-114">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="1d45d-114">Allow the user to set.</span></span>|
|<span data-ttu-id="1d45d-115">all</span><span class="sxs-lookup"><span data-stu-id="1d45d-115">all</span></span>|<span data-ttu-id="1d45d-116">1</span><span class="sxs-lookup"><span data-stu-id="1d45d-116">1</span></span>|<span data-ttu-id="1d45d-117">半年 （目标） 通道。</span><span class="sxs-lookup"><span data-stu-id="1d45d-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="1d45d-118">设备从半年通道 （目标） 中获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="1d45d-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="1d45d-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="1d45d-119">businessReadyOnly</span></span>|<span data-ttu-id="1d45d-120">2</span><span class="sxs-lookup"><span data-stu-id="1d45d-120">2</span></span>|<span data-ttu-id="1d45d-121">半年通道。</span><span class="sxs-lookup"><span data-stu-id="1d45d-121">Semi-annual Channel.</span></span> <span data-ttu-id="1d45d-122">设备获取更新功能从半年通道。</span><span class="sxs-lookup"><span data-stu-id="1d45d-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="1d45d-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="1d45d-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="1d45d-124">3</span><span class="sxs-lookup"><span data-stu-id="1d45d-124">3</span></span>|<span data-ttu-id="1d45d-125">Windows 内幕生成-Fast</span><span class="sxs-lookup"><span data-stu-id="1d45d-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="1d45d-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="1d45d-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="1d45d-127">4</span><span class="sxs-lookup"><span data-stu-id="1d45d-127">4</span></span>|<span data-ttu-id="1d45d-128">Windows 内幕生成-速度较慢</span><span class="sxs-lookup"><span data-stu-id="1d45d-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="1d45d-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="1d45d-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="1d45d-130">5</span><span class="sxs-lookup"><span data-stu-id="1d45d-130">5</span></span>|<span data-ttu-id="1d45d-131">Windows 内幕发布版本</span><span class="sxs-lookup"><span data-stu-id="1d45d-131">Release Windows Insider build</span></span>|





