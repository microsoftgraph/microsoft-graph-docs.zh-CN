---
title: actionState 枚举类型
description: 在设备上的操作的状态
author: tfitzmac
ms.openlocfilehash: 1f36c3a6709ade5860ff24cc8d10c2cb0294a471
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315104"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="fb603-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fb603-103">actionState enum type</span></span>

> <span data-ttu-id="fb603-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb603-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb603-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb603-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb603-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fb603-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb603-107">在设备上的操作的状态</span><span class="sxs-lookup"><span data-stu-id="fb603-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="fb603-108">成员</span><span class="sxs-lookup"><span data-stu-id="fb603-108">Members</span></span>
|<span data-ttu-id="fb603-109">成员</span><span class="sxs-lookup"><span data-stu-id="fb603-109">Member</span></span>|<span data-ttu-id="fb603-110">值</span><span class="sxs-lookup"><span data-stu-id="fb603-110">Value</span></span>|<span data-ttu-id="fb603-111">说明</span><span class="sxs-lookup"><span data-stu-id="fb603-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb603-112">无</span><span class="sxs-lookup"><span data-stu-id="fb603-112">none</span></span>|<span data-ttu-id="fb603-113">0</span><span class="sxs-lookup"><span data-stu-id="fb603-113">0</span></span>|<span data-ttu-id="fb603-114">不是有效的操作状态</span><span class="sxs-lookup"><span data-stu-id="fb603-114">Not a valid action state</span></span>|
|<span data-ttu-id="fb603-115">挂起</span><span class="sxs-lookup"><span data-stu-id="fb603-115">pending</span></span>|<span data-ttu-id="fb603-116">1</span><span class="sxs-lookup"><span data-stu-id="fb603-116">1</span></span>|<span data-ttu-id="fb603-117">操作处于挂起状态</span><span class="sxs-lookup"><span data-stu-id="fb603-117">Action is pending</span></span>|
|<span data-ttu-id="fb603-118">取消此事件</span><span class="sxs-lookup"><span data-stu-id="fb603-118">canceled</span></span>|<span data-ttu-id="fb603-119">2</span><span class="sxs-lookup"><span data-stu-id="fb603-119">2</span></span>|<span data-ttu-id="fb603-120">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="fb603-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="fb603-121">活动</span><span class="sxs-lookup"><span data-stu-id="fb603-121">active</span></span>|<span data-ttu-id="fb603-122">3</span><span class="sxs-lookup"><span data-stu-id="fb603-122">3</span></span>|<span data-ttu-id="fb603-123">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="fb603-123">Action is active.</span></span>|
|<span data-ttu-id="fb603-124">done</span><span class="sxs-lookup"><span data-stu-id="fb603-124">done</span></span>|<span data-ttu-id="fb603-125">4</span><span class="sxs-lookup"><span data-stu-id="fb603-125">4</span></span>|<span data-ttu-id="fb603-126">没有错误完成的操作。</span><span class="sxs-lookup"><span data-stu-id="fb603-126">Action completed without errors.</span></span>|
|<span data-ttu-id="fb603-127">failed</span><span class="sxs-lookup"><span data-stu-id="fb603-127">failed</span></span>|<span data-ttu-id="fb603-128">5</span><span class="sxs-lookup"><span data-stu-id="fb603-128">5</span></span>|<span data-ttu-id="fb603-129">失败的操作</span><span class="sxs-lookup"><span data-stu-id="fb603-129">Action failed</span></span>|
|<span data-ttu-id="fb603-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="fb603-130">notSupported</span></span>|<span data-ttu-id="fb603-131">6</span><span class="sxs-lookup"><span data-stu-id="fb603-131">6</span></span>|<span data-ttu-id="fb603-132">不支持操作。</span><span class="sxs-lookup"><span data-stu-id="fb603-132">Action is not supported.</span></span>|





