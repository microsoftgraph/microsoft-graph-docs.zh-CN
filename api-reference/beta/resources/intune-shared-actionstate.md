---
title: actionState 枚举类型
description: 在设备上的操作的状态
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14ec93848deccb7d6bb21331095f9ecf4a881815
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990850"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="00b52-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="00b52-103">actionState enum type</span></span>

> <span data-ttu-id="00b52-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="00b52-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00b52-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00b52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00b52-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="00b52-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00b52-107">在设备上的操作的状态</span><span class="sxs-lookup"><span data-stu-id="00b52-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="00b52-108">成员</span><span class="sxs-lookup"><span data-stu-id="00b52-108">Members</span></span>
|<span data-ttu-id="00b52-109">成员</span><span class="sxs-lookup"><span data-stu-id="00b52-109">Member</span></span>|<span data-ttu-id="00b52-110">值</span><span class="sxs-lookup"><span data-stu-id="00b52-110">Value</span></span>|<span data-ttu-id="00b52-111">说明</span><span class="sxs-lookup"><span data-stu-id="00b52-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00b52-112">无</span><span class="sxs-lookup"><span data-stu-id="00b52-112">none</span></span>|<span data-ttu-id="00b52-113">0</span><span class="sxs-lookup"><span data-stu-id="00b52-113">0</span></span>|<span data-ttu-id="00b52-114">不是有效的操作状态</span><span class="sxs-lookup"><span data-stu-id="00b52-114">Not a valid action state</span></span>|
|<span data-ttu-id="00b52-115">挂起</span><span class="sxs-lookup"><span data-stu-id="00b52-115">pending</span></span>|<span data-ttu-id="00b52-116">1</span><span class="sxs-lookup"><span data-stu-id="00b52-116">1</span></span>|<span data-ttu-id="00b52-117">操作处于挂起状态</span><span class="sxs-lookup"><span data-stu-id="00b52-117">Action is pending</span></span>|
|<span data-ttu-id="00b52-118">取消此事件</span><span class="sxs-lookup"><span data-stu-id="00b52-118">canceled</span></span>|<span data-ttu-id="00b52-119">2</span><span class="sxs-lookup"><span data-stu-id="00b52-119">2</span></span>|<span data-ttu-id="00b52-120">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="00b52-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="00b52-121">活动</span><span class="sxs-lookup"><span data-stu-id="00b52-121">active</span></span>|<span data-ttu-id="00b52-122">3</span><span class="sxs-lookup"><span data-stu-id="00b52-122">3</span></span>|<span data-ttu-id="00b52-123">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="00b52-123">Action is active.</span></span>|
|<span data-ttu-id="00b52-124">done</span><span class="sxs-lookup"><span data-stu-id="00b52-124">done</span></span>|<span data-ttu-id="00b52-125">4</span><span class="sxs-lookup"><span data-stu-id="00b52-125">4</span></span>|<span data-ttu-id="00b52-126">没有错误完成的操作。</span><span class="sxs-lookup"><span data-stu-id="00b52-126">Action completed without errors.</span></span>|
|<span data-ttu-id="00b52-127">failed</span><span class="sxs-lookup"><span data-stu-id="00b52-127">failed</span></span>|<span data-ttu-id="00b52-128">5</span><span class="sxs-lookup"><span data-stu-id="00b52-128">5</span></span>|<span data-ttu-id="00b52-129">失败的操作</span><span class="sxs-lookup"><span data-stu-id="00b52-129">Action failed</span></span>|
|<span data-ttu-id="00b52-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="00b52-130">notSupported</span></span>|<span data-ttu-id="00b52-131">6</span><span class="sxs-lookup"><span data-stu-id="00b52-131">6</span></span>|<span data-ttu-id="00b52-132">不支持操作。</span><span class="sxs-lookup"><span data-stu-id="00b52-132">Action is not supported.</span></span>|





