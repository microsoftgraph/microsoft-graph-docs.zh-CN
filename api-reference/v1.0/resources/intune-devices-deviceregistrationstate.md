---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 89be71ded6aa970a5b1b598fe75488423b2b7de6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532205"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="5b289-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5b289-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="5b289-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b289-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b289-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b289-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b289-106">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="5b289-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="5b289-107">成员</span><span class="sxs-lookup"><span data-stu-id="5b289-107">Members</span></span>
|<span data-ttu-id="5b289-108">成员</span><span class="sxs-lookup"><span data-stu-id="5b289-108">Member</span></span>|<span data-ttu-id="5b289-109">值</span><span class="sxs-lookup"><span data-stu-id="5b289-109">Value</span></span>|<span data-ttu-id="5b289-110">说明</span><span class="sxs-lookup"><span data-stu-id="5b289-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b289-111">notRegistered</span><span class="sxs-lookup"><span data-stu-id="5b289-111">notRegistered</span></span>|<span data-ttu-id="5b289-112">0</span><span class="sxs-lookup"><span data-stu-id="5b289-112">0</span></span>|<span data-ttu-id="5b289-113">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="5b289-113">The device is not registered.</span></span>|
|<span data-ttu-id="5b289-114">注册</span><span class="sxs-lookup"><span data-stu-id="5b289-114">registered</span></span>|<span data-ttu-id="5b289-115">2 </span><span class="sxs-lookup"><span data-stu-id="5b289-115">2</span></span>|<span data-ttu-id="5b289-116">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="5b289-116">The device is registered.</span></span>|
|<span data-ttu-id="5b289-117">吊销</span><span class="sxs-lookup"><span data-stu-id="5b289-117">revoked</span></span>|<span data-ttu-id="5b289-118">3 </span><span class="sxs-lookup"><span data-stu-id="5b289-118">3</span></span>|<span data-ttu-id="5b289-119">设备已被阻止、已擦除或已停用。</span><span class="sxs-lookup"><span data-stu-id="5b289-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="5b289-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="5b289-120">keyConflict</span></span>|<span data-ttu-id="5b289-121">4 </span><span class="sxs-lookup"><span data-stu-id="5b289-121">4</span></span>|<span data-ttu-id="5b289-122">设备有键冲突。</span><span class="sxs-lookup"><span data-stu-id="5b289-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="5b289-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="5b289-123">approvalPending</span></span>|<span data-ttu-id="5b289-124">5 </span><span class="sxs-lookup"><span data-stu-id="5b289-124">5</span></span>|<span data-ttu-id="5b289-125">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="5b289-125">The device is pending approval.</span></span>|
|<span data-ttu-id="5b289-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="5b289-126">certificateReset</span></span>|<span data-ttu-id="5b289-127">6 </span><span class="sxs-lookup"><span data-stu-id="5b289-127">6</span></span>|<span data-ttu-id="5b289-128">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="5b289-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="5b289-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="5b289-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="5b289-130">7 </span><span class="sxs-lookup"><span data-stu-id="5b289-130">7</span></span>|<span data-ttu-id="5b289-131">设备未注册且未完成注册。</span><span class="sxs-lookup"><span data-stu-id="5b289-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="5b289-132">unknown</span><span class="sxs-lookup"><span data-stu-id="5b289-132">unknown</span></span>|<span data-ttu-id="5b289-133">8 </span><span class="sxs-lookup"><span data-stu-id="5b289-133">8</span></span>|<span data-ttu-id="5b289-134">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="5b289-134">The device registration status is unknown.</span></span>|




