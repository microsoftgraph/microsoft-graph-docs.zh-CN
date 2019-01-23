---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90f2dc7f8c11940fa01047d8c61f23c8f0389ed8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396754"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="88eb4-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="88eb4-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="88eb4-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="88eb4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88eb4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88eb4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88eb4-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88eb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88eb4-107">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="88eb4-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="88eb4-108">成员</span><span class="sxs-lookup"><span data-stu-id="88eb4-108">Members</span></span>
|<span data-ttu-id="88eb4-109">成员</span><span class="sxs-lookup"><span data-stu-id="88eb4-109">Member</span></span>|<span data-ttu-id="88eb4-110">值</span><span class="sxs-lookup"><span data-stu-id="88eb4-110">Value</span></span>|<span data-ttu-id="88eb4-111">说明</span><span class="sxs-lookup"><span data-stu-id="88eb4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88eb4-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="88eb4-112">notRegistered</span></span>|<span data-ttu-id="88eb4-113">0</span><span class="sxs-lookup"><span data-stu-id="88eb4-113">0</span></span>|<span data-ttu-id="88eb4-114">未注册设备。</span><span class="sxs-lookup"><span data-stu-id="88eb4-114">The device is not registered.</span></span>|
|<span data-ttu-id="88eb4-115">注册</span><span class="sxs-lookup"><span data-stu-id="88eb4-115">registered</span></span>|<span data-ttu-id="88eb4-116">2</span><span class="sxs-lookup"><span data-stu-id="88eb4-116">2</span></span>|<span data-ttu-id="88eb4-117">已注册设备。</span><span class="sxs-lookup"><span data-stu-id="88eb4-117">The device is registered.</span></span>|
|<span data-ttu-id="88eb4-118">吊销</span><span class="sxs-lookup"><span data-stu-id="88eb4-118">revoked</span></span>|<span data-ttu-id="88eb4-119">3</span><span class="sxs-lookup"><span data-stu-id="88eb4-119">3</span></span>|<span data-ttu-id="88eb4-120">已阻止、 擦除或停用该设备。</span><span class="sxs-lookup"><span data-stu-id="88eb4-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="88eb4-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="88eb4-121">keyConflict</span></span>|<span data-ttu-id="88eb4-122">4</span><span class="sxs-lookup"><span data-stu-id="88eb4-122">4</span></span>|<span data-ttu-id="88eb4-123">设备具有键冲突。</span><span class="sxs-lookup"><span data-stu-id="88eb4-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="88eb4-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="88eb4-124">approvalPending</span></span>|<span data-ttu-id="88eb4-125">5</span><span class="sxs-lookup"><span data-stu-id="88eb4-125">5</span></span>|<span data-ttu-id="88eb4-126">设备是待审批状态。</span><span class="sxs-lookup"><span data-stu-id="88eb4-126">The device is pending approval.</span></span>|
|<span data-ttu-id="88eb4-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="88eb4-127">certificateReset</span></span>|<span data-ttu-id="88eb4-128">6</span><span class="sxs-lookup"><span data-stu-id="88eb4-128">6</span></span>|<span data-ttu-id="88eb4-129">设备证书已被重置。</span><span class="sxs-lookup"><span data-stu-id="88eb4-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="88eb4-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="88eb4-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="88eb4-131">7</span><span class="sxs-lookup"><span data-stu-id="88eb4-131">7</span></span>|<span data-ttu-id="88eb4-132">未注册设备以及待处理的注册。</span><span class="sxs-lookup"><span data-stu-id="88eb4-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="88eb4-133">unknown</span><span class="sxs-lookup"><span data-stu-id="88eb4-133">unknown</span></span>|<span data-ttu-id="88eb4-134">8</span><span class="sxs-lookup"><span data-stu-id="88eb4-134">8</span></span>|<span data-ttu-id="88eb4-135">未知设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="88eb4-135">The device registration status is unknown.</span></span>|




