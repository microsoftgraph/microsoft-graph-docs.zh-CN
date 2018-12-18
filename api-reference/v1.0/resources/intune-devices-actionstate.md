---
title: actionState 枚举类型
description: 在设备上的操作的状态
author: tfitzmac
ms.openlocfilehash: 53ee72430ac646bf978a3167b87feaf398c8ac37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333381"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="3ea36-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3ea36-103">actionState enum type</span></span>

> <span data-ttu-id="3ea36-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3ea36-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ea36-105">在设备上的操作的状态</span><span class="sxs-lookup"><span data-stu-id="3ea36-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="3ea36-106">成员</span><span class="sxs-lookup"><span data-stu-id="3ea36-106">Members</span></span>
|<span data-ttu-id="3ea36-107">成员</span><span class="sxs-lookup"><span data-stu-id="3ea36-107">Member</span></span>|<span data-ttu-id="3ea36-108">值</span><span class="sxs-lookup"><span data-stu-id="3ea36-108">Value</span></span>|<span data-ttu-id="3ea36-109">说明</span><span class="sxs-lookup"><span data-stu-id="3ea36-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ea36-110">无</span><span class="sxs-lookup"><span data-stu-id="3ea36-110">none</span></span>|<span data-ttu-id="3ea36-111">0</span><span class="sxs-lookup"><span data-stu-id="3ea36-111">0</span></span>|<span data-ttu-id="3ea36-112">不是有效的操作状态</span><span class="sxs-lookup"><span data-stu-id="3ea36-112">Not a valid action state</span></span>|
|<span data-ttu-id="3ea36-113">挂起</span><span class="sxs-lookup"><span data-stu-id="3ea36-113">pending</span></span>|<span data-ttu-id="3ea36-114">1</span><span class="sxs-lookup"><span data-stu-id="3ea36-114">1</span></span>|<span data-ttu-id="3ea36-115">操作处于挂起状态</span><span class="sxs-lookup"><span data-stu-id="3ea36-115">Action is pending</span></span>|
|<span data-ttu-id="3ea36-116">取消此事件</span><span class="sxs-lookup"><span data-stu-id="3ea36-116">canceled</span></span>|<span data-ttu-id="3ea36-117">2</span><span class="sxs-lookup"><span data-stu-id="3ea36-117">2</span></span>|<span data-ttu-id="3ea36-118">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="3ea36-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="3ea36-119">活动</span><span class="sxs-lookup"><span data-stu-id="3ea36-119">active</span></span>|<span data-ttu-id="3ea36-120">3</span><span class="sxs-lookup"><span data-stu-id="3ea36-120">3</span></span>|<span data-ttu-id="3ea36-121">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="3ea36-121">Action is active.</span></span>|
|<span data-ttu-id="3ea36-122">done</span><span class="sxs-lookup"><span data-stu-id="3ea36-122">done</span></span>|<span data-ttu-id="3ea36-123">4</span><span class="sxs-lookup"><span data-stu-id="3ea36-123">4</span></span>|<span data-ttu-id="3ea36-124">没有错误完成的操作。</span><span class="sxs-lookup"><span data-stu-id="3ea36-124">Action completed without errors.</span></span>|
|<span data-ttu-id="3ea36-125">failed</span><span class="sxs-lookup"><span data-stu-id="3ea36-125">failed</span></span>|<span data-ttu-id="3ea36-126">5</span><span class="sxs-lookup"><span data-stu-id="3ea36-126">5</span></span>|<span data-ttu-id="3ea36-127">失败的操作</span><span class="sxs-lookup"><span data-stu-id="3ea36-127">Action failed</span></span>|
|<span data-ttu-id="3ea36-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="3ea36-128">notSupported</span></span>|<span data-ttu-id="3ea36-129">6</span><span class="sxs-lookup"><span data-stu-id="3ea36-129">6</span></span>|<span data-ttu-id="3ea36-130">不支持操作。</span><span class="sxs-lookup"><span data-stu-id="3ea36-130">Action is not supported.</span></span>|



