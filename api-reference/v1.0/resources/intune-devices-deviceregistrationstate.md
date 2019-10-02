---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2543f1a7d874a8443424fa1161187e7ccd771f7b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356917"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="ca21c-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ca21c-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="ca21c-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca21c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca21c-105">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="ca21c-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="ca21c-106">成员</span><span class="sxs-lookup"><span data-stu-id="ca21c-106">Members</span></span>
|<span data-ttu-id="ca21c-107">成员</span><span class="sxs-lookup"><span data-stu-id="ca21c-107">Member</span></span>|<span data-ttu-id="ca21c-108">值</span><span class="sxs-lookup"><span data-stu-id="ca21c-108">Value</span></span>|<span data-ttu-id="ca21c-109">说明</span><span class="sxs-lookup"><span data-stu-id="ca21c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca21c-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="ca21c-110">notRegistered</span></span>|<span data-ttu-id="ca21c-111">0</span><span class="sxs-lookup"><span data-stu-id="ca21c-111">0</span></span>|<span data-ttu-id="ca21c-112">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="ca21c-112">The device is not registered.</span></span>|
|<span data-ttu-id="ca21c-113">注册</span><span class="sxs-lookup"><span data-stu-id="ca21c-113">registered</span></span>|<span data-ttu-id="ca21c-114">双面</span><span class="sxs-lookup"><span data-stu-id="ca21c-114">2</span></span>|<span data-ttu-id="ca21c-115">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="ca21c-115">The device is registered.</span></span>|
|<span data-ttu-id="ca21c-116">吊销</span><span class="sxs-lookup"><span data-stu-id="ca21c-116">revoked</span></span>|<span data-ttu-id="ca21c-117">第三章</span><span class="sxs-lookup"><span data-stu-id="ca21c-117">3</span></span>|<span data-ttu-id="ca21c-118">设备已被阻止、已擦除或已停用。</span><span class="sxs-lookup"><span data-stu-id="ca21c-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="ca21c-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="ca21c-119">keyConflict</span></span>|<span data-ttu-id="ca21c-120">4</span><span class="sxs-lookup"><span data-stu-id="ca21c-120">4</span></span>|<span data-ttu-id="ca21c-121">设备有键冲突。</span><span class="sxs-lookup"><span data-stu-id="ca21c-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="ca21c-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="ca21c-122">approvalPending</span></span>|<span data-ttu-id="ca21c-123">5</span><span class="sxs-lookup"><span data-stu-id="ca21c-123">5</span></span>|<span data-ttu-id="ca21c-124">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="ca21c-124">The device is pending approval.</span></span>|
|<span data-ttu-id="ca21c-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="ca21c-125">certificateReset</span></span>|<span data-ttu-id="ca21c-126">型</span><span class="sxs-lookup"><span data-stu-id="ca21c-126">6</span></span>|<span data-ttu-id="ca21c-127">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="ca21c-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="ca21c-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="ca21c-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="ca21c-129">步</span><span class="sxs-lookup"><span data-stu-id="ca21c-129">7</span></span>|<span data-ttu-id="ca21c-130">设备未注册且未完成注册。</span><span class="sxs-lookup"><span data-stu-id="ca21c-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="ca21c-131">unknown</span><span class="sxs-lookup"><span data-stu-id="ca21c-131">unknown</span></span>|<span data-ttu-id="ca21c-132">utf-8</span><span class="sxs-lookup"><span data-stu-id="ca21c-132">8</span></span>|<span data-ttu-id="ca21c-133">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="ca21c-133">The device registration status is unknown.</span></span>|




