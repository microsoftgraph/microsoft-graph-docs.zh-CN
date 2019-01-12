---
title: actionState 枚举类型
description: 在设备上的操作的状态
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5579d8de986a764cd96e42dff30c007449130b0b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922443"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="5d78d-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5d78d-103">actionState enum type</span></span>

> <span data-ttu-id="5d78d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5d78d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d78d-105">在设备上的操作的状态</span><span class="sxs-lookup"><span data-stu-id="5d78d-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="5d78d-106">成员</span><span class="sxs-lookup"><span data-stu-id="5d78d-106">Members</span></span>
|<span data-ttu-id="5d78d-107">成员</span><span class="sxs-lookup"><span data-stu-id="5d78d-107">Member</span></span>|<span data-ttu-id="5d78d-108">值</span><span class="sxs-lookup"><span data-stu-id="5d78d-108">Value</span></span>|<span data-ttu-id="5d78d-109">Description</span><span class="sxs-lookup"><span data-stu-id="5d78d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d78d-110">无</span><span class="sxs-lookup"><span data-stu-id="5d78d-110">none</span></span>|<span data-ttu-id="5d78d-111">0</span><span class="sxs-lookup"><span data-stu-id="5d78d-111">0</span></span>|<span data-ttu-id="5d78d-112">不是有效的操作状态</span><span class="sxs-lookup"><span data-stu-id="5d78d-112">Not a valid action state</span></span>|
|<span data-ttu-id="5d78d-113">挂起</span><span class="sxs-lookup"><span data-stu-id="5d78d-113">pending</span></span>|<span data-ttu-id="5d78d-114">1</span><span class="sxs-lookup"><span data-stu-id="5d78d-114">1</span></span>|<span data-ttu-id="5d78d-115">操作处于挂起状态</span><span class="sxs-lookup"><span data-stu-id="5d78d-115">Action is pending</span></span>|
|<span data-ttu-id="5d78d-116">取消此事件</span><span class="sxs-lookup"><span data-stu-id="5d78d-116">canceled</span></span>|<span data-ttu-id="5d78d-117">2</span><span class="sxs-lookup"><span data-stu-id="5d78d-117">2</span></span>|<span data-ttu-id="5d78d-118">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="5d78d-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="5d78d-119">活动</span><span class="sxs-lookup"><span data-stu-id="5d78d-119">active</span></span>|<span data-ttu-id="5d78d-120">3</span><span class="sxs-lookup"><span data-stu-id="5d78d-120">3</span></span>|<span data-ttu-id="5d78d-121">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="5d78d-121">Action is active.</span></span>|
|<span data-ttu-id="5d78d-122">done</span><span class="sxs-lookup"><span data-stu-id="5d78d-122">done</span></span>|<span data-ttu-id="5d78d-123">4</span><span class="sxs-lookup"><span data-stu-id="5d78d-123">4</span></span>|<span data-ttu-id="5d78d-124">没有错误完成的操作。</span><span class="sxs-lookup"><span data-stu-id="5d78d-124">Action completed without errors.</span></span>|
|<span data-ttu-id="5d78d-125">failed</span><span class="sxs-lookup"><span data-stu-id="5d78d-125">failed</span></span>|<span data-ttu-id="5d78d-126">5</span><span class="sxs-lookup"><span data-stu-id="5d78d-126">5</span></span>|<span data-ttu-id="5d78d-127">失败的操作</span><span class="sxs-lookup"><span data-stu-id="5d78d-127">Action failed</span></span>|
|<span data-ttu-id="5d78d-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="5d78d-128">notSupported</span></span>|<span data-ttu-id="5d78d-129">6</span><span class="sxs-lookup"><span data-stu-id="5d78d-129">6</span></span>|<span data-ttu-id="5d78d-130">不支持操作。</span><span class="sxs-lookup"><span data-stu-id="5d78d-130">Action is not supported.</span></span>|



