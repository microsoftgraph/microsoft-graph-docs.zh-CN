---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580972"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="e978e-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e978e-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="e978e-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e978e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e978e-105">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="e978e-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="e978e-106">成员</span><span class="sxs-lookup"><span data-stu-id="e978e-106">Members</span></span>
|<span data-ttu-id="e978e-107">成员</span><span class="sxs-lookup"><span data-stu-id="e978e-107">Member</span></span>|<span data-ttu-id="e978e-108">值</span><span class="sxs-lookup"><span data-stu-id="e978e-108">Value</span></span>|<span data-ttu-id="e978e-109">说明</span><span class="sxs-lookup"><span data-stu-id="e978e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e978e-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="e978e-110">notRegistered</span></span>|<span data-ttu-id="e978e-111">0</span><span class="sxs-lookup"><span data-stu-id="e978e-111">0</span></span>|<span data-ttu-id="e978e-112">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="e978e-112">The device is not registered.</span></span>|
|<span data-ttu-id="e978e-113">注册</span><span class="sxs-lookup"><span data-stu-id="e978e-113">registered</span></span>|<span data-ttu-id="e978e-114">2 </span><span class="sxs-lookup"><span data-stu-id="e978e-114">2</span></span>|<span data-ttu-id="e978e-115">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="e978e-115">The device is registered.</span></span>|
|<span data-ttu-id="e978e-116">吊销</span><span class="sxs-lookup"><span data-stu-id="e978e-116">revoked</span></span>|<span data-ttu-id="e978e-117">3 </span><span class="sxs-lookup"><span data-stu-id="e978e-117">3</span></span>|<span data-ttu-id="e978e-118">设备已被阻止、已擦除或已停用。</span><span class="sxs-lookup"><span data-stu-id="e978e-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="e978e-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="e978e-119">keyConflict</span></span>|<span data-ttu-id="e978e-120">4 </span><span class="sxs-lookup"><span data-stu-id="e978e-120">4</span></span>|<span data-ttu-id="e978e-121">设备有键冲突。</span><span class="sxs-lookup"><span data-stu-id="e978e-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="e978e-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="e978e-122">approvalPending</span></span>|<span data-ttu-id="e978e-123">5 </span><span class="sxs-lookup"><span data-stu-id="e978e-123">5</span></span>|<span data-ttu-id="e978e-124">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="e978e-124">The device is pending approval.</span></span>|
|<span data-ttu-id="e978e-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="e978e-125">certificateReset</span></span>|<span data-ttu-id="e978e-126">6 </span><span class="sxs-lookup"><span data-stu-id="e978e-126">6</span></span>|<span data-ttu-id="e978e-127">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="e978e-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="e978e-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="e978e-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="e978e-129">7 </span><span class="sxs-lookup"><span data-stu-id="e978e-129">7</span></span>|<span data-ttu-id="e978e-130">设备未注册且未完成注册。</span><span class="sxs-lookup"><span data-stu-id="e978e-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="e978e-131">unknown</span><span class="sxs-lookup"><span data-stu-id="e978e-131">unknown</span></span>|<span data-ttu-id="e978e-132">8 </span><span class="sxs-lookup"><span data-stu-id="e978e-132">8</span></span>|<span data-ttu-id="e978e-133">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="e978e-133">The device registration status is unknown.</span></span>|



