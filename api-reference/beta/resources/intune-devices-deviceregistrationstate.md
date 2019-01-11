---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7633419ebeeb5c5865cd1a80c251effbf314b018
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829762"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="ff59a-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ff59a-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="ff59a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ff59a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff59a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ff59a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff59a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ff59a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff59a-107">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="ff59a-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="ff59a-108">成员</span><span class="sxs-lookup"><span data-stu-id="ff59a-108">Members</span></span>
|<span data-ttu-id="ff59a-109">成员</span><span class="sxs-lookup"><span data-stu-id="ff59a-109">Member</span></span>|<span data-ttu-id="ff59a-110">值</span><span class="sxs-lookup"><span data-stu-id="ff59a-110">Value</span></span>|<span data-ttu-id="ff59a-111">Description</span><span class="sxs-lookup"><span data-stu-id="ff59a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff59a-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="ff59a-112">notRegistered</span></span>|<span data-ttu-id="ff59a-113">0</span><span class="sxs-lookup"><span data-stu-id="ff59a-113">0</span></span>|<span data-ttu-id="ff59a-114">未注册设备。</span><span class="sxs-lookup"><span data-stu-id="ff59a-114">The device is not registered.</span></span>|
|<span data-ttu-id="ff59a-115">注册</span><span class="sxs-lookup"><span data-stu-id="ff59a-115">registered</span></span>|<span data-ttu-id="ff59a-116">2</span><span class="sxs-lookup"><span data-stu-id="ff59a-116">2</span></span>|<span data-ttu-id="ff59a-117">已注册设备。</span><span class="sxs-lookup"><span data-stu-id="ff59a-117">The device is registered.</span></span>|
|<span data-ttu-id="ff59a-118">吊销</span><span class="sxs-lookup"><span data-stu-id="ff59a-118">revoked</span></span>|<span data-ttu-id="ff59a-119">3</span><span class="sxs-lookup"><span data-stu-id="ff59a-119">3</span></span>|<span data-ttu-id="ff59a-120">已阻止、 擦除或停用该设备。</span><span class="sxs-lookup"><span data-stu-id="ff59a-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="ff59a-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="ff59a-121">keyConflict</span></span>|<span data-ttu-id="ff59a-122">4</span><span class="sxs-lookup"><span data-stu-id="ff59a-122">4</span></span>|<span data-ttu-id="ff59a-123">设备具有键冲突。</span><span class="sxs-lookup"><span data-stu-id="ff59a-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="ff59a-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="ff59a-124">approvalPending</span></span>|<span data-ttu-id="ff59a-125">5</span><span class="sxs-lookup"><span data-stu-id="ff59a-125">5</span></span>|<span data-ttu-id="ff59a-126">设备是待审批状态。</span><span class="sxs-lookup"><span data-stu-id="ff59a-126">The device is pending approval.</span></span>|
|<span data-ttu-id="ff59a-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="ff59a-127">certificateReset</span></span>|<span data-ttu-id="ff59a-128">6</span><span class="sxs-lookup"><span data-stu-id="ff59a-128">6</span></span>|<span data-ttu-id="ff59a-129">设备证书已被重置。</span><span class="sxs-lookup"><span data-stu-id="ff59a-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="ff59a-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="ff59a-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="ff59a-131">7</span><span class="sxs-lookup"><span data-stu-id="ff59a-131">7</span></span>|<span data-ttu-id="ff59a-132">未注册设备以及待处理的注册。</span><span class="sxs-lookup"><span data-stu-id="ff59a-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="ff59a-133">unknown</span><span class="sxs-lookup"><span data-stu-id="ff59a-133">unknown</span></span>|<span data-ttu-id="ff59a-134">8</span><span class="sxs-lookup"><span data-stu-id="ff59a-134">8</span></span>|<span data-ttu-id="ff59a-135">未知设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="ff59a-135">The device registration status is unknown.</span></span>|





