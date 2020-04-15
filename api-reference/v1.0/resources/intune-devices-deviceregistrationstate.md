---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b1974d8124c834185617332096d6b44429c7900a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472421"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="fabbd-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fabbd-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="fabbd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fabbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fabbd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fabbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fabbd-106">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="fabbd-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="fabbd-107">成员</span><span class="sxs-lookup"><span data-stu-id="fabbd-107">Members</span></span>
|<span data-ttu-id="fabbd-108">成员</span><span class="sxs-lookup"><span data-stu-id="fabbd-108">Member</span></span>|<span data-ttu-id="fabbd-109">值</span><span class="sxs-lookup"><span data-stu-id="fabbd-109">Value</span></span>|<span data-ttu-id="fabbd-110">说明</span><span class="sxs-lookup"><span data-stu-id="fabbd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fabbd-111">notRegistered</span><span class="sxs-lookup"><span data-stu-id="fabbd-111">notRegistered</span></span>|<span data-ttu-id="fabbd-112">0</span><span class="sxs-lookup"><span data-stu-id="fabbd-112">0</span></span>|<span data-ttu-id="fabbd-113">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="fabbd-113">The device is not registered.</span></span>|
|<span data-ttu-id="fabbd-114">注册</span><span class="sxs-lookup"><span data-stu-id="fabbd-114">registered</span></span>|<span data-ttu-id="fabbd-115">双面</span><span class="sxs-lookup"><span data-stu-id="fabbd-115">2</span></span>|<span data-ttu-id="fabbd-116">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="fabbd-116">The device is registered.</span></span>|
|<span data-ttu-id="fabbd-117">吊销</span><span class="sxs-lookup"><span data-stu-id="fabbd-117">revoked</span></span>|<span data-ttu-id="fabbd-118">第三章</span><span class="sxs-lookup"><span data-stu-id="fabbd-118">3</span></span>|<span data-ttu-id="fabbd-119">设备已被阻止、已擦除或已停用。</span><span class="sxs-lookup"><span data-stu-id="fabbd-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="fabbd-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="fabbd-120">keyConflict</span></span>|<span data-ttu-id="fabbd-121">4 </span><span class="sxs-lookup"><span data-stu-id="fabbd-121">4</span></span>|<span data-ttu-id="fabbd-122">设备有键冲突。</span><span class="sxs-lookup"><span data-stu-id="fabbd-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="fabbd-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="fabbd-123">approvalPending</span></span>|<span data-ttu-id="fabbd-124">5 </span><span class="sxs-lookup"><span data-stu-id="fabbd-124">5</span></span>|<span data-ttu-id="fabbd-125">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="fabbd-125">The device is pending approval.</span></span>|
|<span data-ttu-id="fabbd-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="fabbd-126">certificateReset</span></span>|<span data-ttu-id="fabbd-127">6 </span><span class="sxs-lookup"><span data-stu-id="fabbd-127">6</span></span>|<span data-ttu-id="fabbd-128">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="fabbd-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="fabbd-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="fabbd-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="fabbd-130">7 </span><span class="sxs-lookup"><span data-stu-id="fabbd-130">7</span></span>|<span data-ttu-id="fabbd-131">设备未注册且未完成注册。</span><span class="sxs-lookup"><span data-stu-id="fabbd-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="fabbd-132">unknown</span><span class="sxs-lookup"><span data-stu-id="fabbd-132">unknown</span></span>|<span data-ttu-id="fabbd-133">8 </span><span class="sxs-lookup"><span data-stu-id="fabbd-133">8</span></span>|<span data-ttu-id="fabbd-134">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="fabbd-134">The device registration status is unknown.</span></span>|







