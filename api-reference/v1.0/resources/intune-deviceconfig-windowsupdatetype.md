---
title: windowsUpdateType 枚举类型
description: 分支的设备将接收从其更新
author: tfitzmac
ms.openlocfilehash: 415dde619529ffa9bb40ab2cea36665558bb0ee9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340836"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="947ff-103">windowsUpdateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="947ff-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="947ff-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="947ff-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="947ff-105">分支的设备将接收从其更新</span><span class="sxs-lookup"><span data-stu-id="947ff-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="947ff-106">成员</span><span class="sxs-lookup"><span data-stu-id="947ff-106">Members</span></span>
|<span data-ttu-id="947ff-107">成员</span><span class="sxs-lookup"><span data-stu-id="947ff-107">Member</span></span>|<span data-ttu-id="947ff-108">值</span><span class="sxs-lookup"><span data-stu-id="947ff-108">Value</span></span>|<span data-ttu-id="947ff-109">说明</span><span class="sxs-lookup"><span data-stu-id="947ff-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="947ff-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="947ff-110">userDefined</span></span>|<span data-ttu-id="947ff-111">0</span><span class="sxs-lookup"><span data-stu-id="947ff-111">0</span></span>|<span data-ttu-id="947ff-112">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="947ff-112">Allow the user to set.</span></span>|
|<span data-ttu-id="947ff-113">all</span><span class="sxs-lookup"><span data-stu-id="947ff-113">all</span></span>|<span data-ttu-id="947ff-114">1</span><span class="sxs-lookup"><span data-stu-id="947ff-114">1</span></span>|<span data-ttu-id="947ff-115">半年 （目标） 通道。</span><span class="sxs-lookup"><span data-stu-id="947ff-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="947ff-116">设备从半年通道 （目标） 中获取所有适用的功能更新。</span><span class="sxs-lookup"><span data-stu-id="947ff-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="947ff-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="947ff-117">businessReadyOnly</span></span>|<span data-ttu-id="947ff-118">2</span><span class="sxs-lookup"><span data-stu-id="947ff-118">2</span></span>|<span data-ttu-id="947ff-119">半年通道。</span><span class="sxs-lookup"><span data-stu-id="947ff-119">Semi-annual Channel.</span></span> <span data-ttu-id="947ff-120">设备获取更新功能从半年通道。</span><span class="sxs-lookup"><span data-stu-id="947ff-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="947ff-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="947ff-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="947ff-122">3</span><span class="sxs-lookup"><span data-stu-id="947ff-122">3</span></span>|<span data-ttu-id="947ff-123">Windows 内幕生成-Fast</span><span class="sxs-lookup"><span data-stu-id="947ff-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="947ff-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="947ff-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="947ff-125">4</span><span class="sxs-lookup"><span data-stu-id="947ff-125">4</span></span>|<span data-ttu-id="947ff-126">Windows 内幕生成-速度较慢</span><span class="sxs-lookup"><span data-stu-id="947ff-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="947ff-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="947ff-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="947ff-128">5</span><span class="sxs-lookup"><span data-stu-id="947ff-128">5</span></span>|<span data-ttu-id="947ff-129">Windows 内幕发布版本</span><span class="sxs-lookup"><span data-stu-id="947ff-129">Release Windows Insider build</span></span>|



