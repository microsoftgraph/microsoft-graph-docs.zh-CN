---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: tfitzmac
ms.openlocfilehash: a622613bd4ca5e065c3d9eb0331c05c360c1837c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360541"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="771b0-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="771b0-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="771b0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="771b0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="771b0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="771b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="771b0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="771b0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="771b0-107">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="771b0-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="771b0-108">成员</span><span class="sxs-lookup"><span data-stu-id="771b0-108">Members</span></span>
|<span data-ttu-id="771b0-109">成员</span><span class="sxs-lookup"><span data-stu-id="771b0-109">Member</span></span>|<span data-ttu-id="771b0-110">值</span><span class="sxs-lookup"><span data-stu-id="771b0-110">Value</span></span>|<span data-ttu-id="771b0-111">说明</span><span class="sxs-lookup"><span data-stu-id="771b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="771b0-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="771b0-112">notRegistered</span></span>|<span data-ttu-id="771b0-113">0</span><span class="sxs-lookup"><span data-stu-id="771b0-113">0</span></span>|<span data-ttu-id="771b0-114">未注册设备。</span><span class="sxs-lookup"><span data-stu-id="771b0-114">The device is not registered.</span></span>|
|<span data-ttu-id="771b0-115">注册</span><span class="sxs-lookup"><span data-stu-id="771b0-115">registered</span></span>|<span data-ttu-id="771b0-116">2</span><span class="sxs-lookup"><span data-stu-id="771b0-116">2</span></span>|<span data-ttu-id="771b0-117">已注册设备。</span><span class="sxs-lookup"><span data-stu-id="771b0-117">The device is registered.</span></span>|
|<span data-ttu-id="771b0-118">吊销</span><span class="sxs-lookup"><span data-stu-id="771b0-118">revoked</span></span>|<span data-ttu-id="771b0-119">3</span><span class="sxs-lookup"><span data-stu-id="771b0-119">3</span></span>|<span data-ttu-id="771b0-120">已阻止、 擦除或停用该设备。</span><span class="sxs-lookup"><span data-stu-id="771b0-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="771b0-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="771b0-121">keyConflict</span></span>|<span data-ttu-id="771b0-122">4</span><span class="sxs-lookup"><span data-stu-id="771b0-122">4</span></span>|<span data-ttu-id="771b0-123">设备具有键冲突。</span><span class="sxs-lookup"><span data-stu-id="771b0-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="771b0-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="771b0-124">approvalPending</span></span>|<span data-ttu-id="771b0-125">5</span><span class="sxs-lookup"><span data-stu-id="771b0-125">5</span></span>|<span data-ttu-id="771b0-126">设备是待审批状态。</span><span class="sxs-lookup"><span data-stu-id="771b0-126">The device is pending approval.</span></span>|
|<span data-ttu-id="771b0-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="771b0-127">certificateReset</span></span>|<span data-ttu-id="771b0-128">6</span><span class="sxs-lookup"><span data-stu-id="771b0-128">6</span></span>|<span data-ttu-id="771b0-129">设备证书已被重置。</span><span class="sxs-lookup"><span data-stu-id="771b0-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="771b0-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="771b0-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="771b0-131">7</span><span class="sxs-lookup"><span data-stu-id="771b0-131">7</span></span>|<span data-ttu-id="771b0-132">未注册设备以及待处理的注册。</span><span class="sxs-lookup"><span data-stu-id="771b0-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="771b0-133">unknown</span><span class="sxs-lookup"><span data-stu-id="771b0-133">unknown</span></span>|<span data-ttu-id="771b0-134">8</span><span class="sxs-lookup"><span data-stu-id="771b0-134">8</span></span>|<span data-ttu-id="771b0-135">未知设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="771b0-135">The device registration status is unknown.</span></span>|





