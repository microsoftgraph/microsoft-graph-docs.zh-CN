---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b777452b627208d8e2dd726815f321075e5745ae
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794013"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="f5be6-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f5be6-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="f5be6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5be6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5be6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5be6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5be6-106">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="f5be6-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="f5be6-107">成员</span><span class="sxs-lookup"><span data-stu-id="f5be6-107">Members</span></span>
|<span data-ttu-id="f5be6-108">成员</span><span class="sxs-lookup"><span data-stu-id="f5be6-108">Member</span></span>|<span data-ttu-id="f5be6-109">值</span><span class="sxs-lookup"><span data-stu-id="f5be6-109">Value</span></span>|<span data-ttu-id="f5be6-110">说明</span><span class="sxs-lookup"><span data-stu-id="f5be6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5be6-111">notRegistered</span><span class="sxs-lookup"><span data-stu-id="f5be6-111">notRegistered</span></span>|<span data-ttu-id="f5be6-112">0</span><span class="sxs-lookup"><span data-stu-id="f5be6-112">0</span></span>|<span data-ttu-id="f5be6-113">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="f5be6-113">The device is not registered.</span></span>|
|<span data-ttu-id="f5be6-114">注册</span><span class="sxs-lookup"><span data-stu-id="f5be6-114">registered</span></span>|<span data-ttu-id="f5be6-115">双面</span><span class="sxs-lookup"><span data-stu-id="f5be6-115">2</span></span>|<span data-ttu-id="f5be6-116">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="f5be6-116">The device is registered.</span></span>|
|<span data-ttu-id="f5be6-117">吊销</span><span class="sxs-lookup"><span data-stu-id="f5be6-117">revoked</span></span>|<span data-ttu-id="f5be6-118">第三章</span><span class="sxs-lookup"><span data-stu-id="f5be6-118">3</span></span>|<span data-ttu-id="f5be6-119">设备已被阻止、已擦除或已停用。</span><span class="sxs-lookup"><span data-stu-id="f5be6-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="f5be6-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="f5be6-120">keyConflict</span></span>|<span data-ttu-id="f5be6-121">4</span><span class="sxs-lookup"><span data-stu-id="f5be6-121">4</span></span>|<span data-ttu-id="f5be6-122">设备有键冲突。</span><span class="sxs-lookup"><span data-stu-id="f5be6-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="f5be6-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="f5be6-123">approvalPending</span></span>|<span data-ttu-id="f5be6-124">5</span><span class="sxs-lookup"><span data-stu-id="f5be6-124">5</span></span>|<span data-ttu-id="f5be6-125">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="f5be6-125">The device is pending approval.</span></span>|
|<span data-ttu-id="f5be6-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="f5be6-126">certificateReset</span></span>|<span data-ttu-id="f5be6-127">型</span><span class="sxs-lookup"><span data-stu-id="f5be6-127">6</span></span>|<span data-ttu-id="f5be6-128">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="f5be6-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="f5be6-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="f5be6-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="f5be6-130">步</span><span class="sxs-lookup"><span data-stu-id="f5be6-130">7</span></span>|<span data-ttu-id="f5be6-131">设备未注册且未完成注册。</span><span class="sxs-lookup"><span data-stu-id="f5be6-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="f5be6-132">unknown</span><span class="sxs-lookup"><span data-stu-id="f5be6-132">unknown</span></span>|<span data-ttu-id="f5be6-133">utf-8</span><span class="sxs-lookup"><span data-stu-id="f5be6-133">8</span></span>|<span data-ttu-id="f5be6-134">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="f5be6-134">The device registration status is unknown.</span></span>|





