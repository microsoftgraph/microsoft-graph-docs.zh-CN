---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 933ea7cf16421ecadd9bb23b4594d8ca0f5e767b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030728"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="4757c-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4757c-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="4757c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4757c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4757c-105">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="4757c-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="4757c-106">成员</span><span class="sxs-lookup"><span data-stu-id="4757c-106">Members</span></span>
|<span data-ttu-id="4757c-107">成员</span><span class="sxs-lookup"><span data-stu-id="4757c-107">Member</span></span>|<span data-ttu-id="4757c-108">值</span><span class="sxs-lookup"><span data-stu-id="4757c-108">Value</span></span>|<span data-ttu-id="4757c-109">说明</span><span class="sxs-lookup"><span data-stu-id="4757c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4757c-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="4757c-110">notRegistered</span></span>|<span data-ttu-id="4757c-111">0</span><span class="sxs-lookup"><span data-stu-id="4757c-111">0</span></span>|<span data-ttu-id="4757c-112">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="4757c-112">The device is not registered.</span></span>|
|<span data-ttu-id="4757c-113">注册</span><span class="sxs-lookup"><span data-stu-id="4757c-113">registered</span></span>|<span data-ttu-id="4757c-114">双面</span><span class="sxs-lookup"><span data-stu-id="4757c-114">2</span></span>|<span data-ttu-id="4757c-115">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="4757c-115">The device is registered.</span></span>|
|<span data-ttu-id="4757c-116">吊销</span><span class="sxs-lookup"><span data-stu-id="4757c-116">revoked</span></span>|<span data-ttu-id="4757c-117">第三章</span><span class="sxs-lookup"><span data-stu-id="4757c-117">3</span></span>|<span data-ttu-id="4757c-118">设备已被阻止、已擦除或已停用。</span><span class="sxs-lookup"><span data-stu-id="4757c-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="4757c-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="4757c-119">keyConflict</span></span>|<span data-ttu-id="4757c-120">4</span><span class="sxs-lookup"><span data-stu-id="4757c-120">4</span></span>|<span data-ttu-id="4757c-121">设备有键冲突。</span><span class="sxs-lookup"><span data-stu-id="4757c-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="4757c-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="4757c-122">approvalPending</span></span>|<span data-ttu-id="4757c-123">5</span><span class="sxs-lookup"><span data-stu-id="4757c-123">5</span></span>|<span data-ttu-id="4757c-124">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="4757c-124">The device is pending approval.</span></span>|
|<span data-ttu-id="4757c-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="4757c-125">certificateReset</span></span>|<span data-ttu-id="4757c-126">型</span><span class="sxs-lookup"><span data-stu-id="4757c-126">6</span></span>|<span data-ttu-id="4757c-127">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="4757c-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="4757c-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="4757c-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="4757c-129">步</span><span class="sxs-lookup"><span data-stu-id="4757c-129">7</span></span>|<span data-ttu-id="4757c-130">设备未注册且未完成注册。</span><span class="sxs-lookup"><span data-stu-id="4757c-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="4757c-131">unknown</span><span class="sxs-lookup"><span data-stu-id="4757c-131">unknown</span></span>|<span data-ttu-id="4757c-132">utf-8</span><span class="sxs-lookup"><span data-stu-id="4757c-132">8</span></span>|<span data-ttu-id="4757c-133">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="4757c-133">The device registration status is unknown.</span></span>|



