---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7aa2f009bc1a9fdafcabbbdbb4a5fbf5d2305b3a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995215"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="6cbff-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6cbff-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="6cbff-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6cbff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cbff-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6cbff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cbff-106">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="6cbff-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="6cbff-107">成员</span><span class="sxs-lookup"><span data-stu-id="6cbff-107">Members</span></span>
|<span data-ttu-id="6cbff-108">成员</span><span class="sxs-lookup"><span data-stu-id="6cbff-108">Member</span></span>|<span data-ttu-id="6cbff-109">值</span><span class="sxs-lookup"><span data-stu-id="6cbff-109">Value</span></span>|<span data-ttu-id="6cbff-110">说明</span><span class="sxs-lookup"><span data-stu-id="6cbff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cbff-111">notRegistered</span><span class="sxs-lookup"><span data-stu-id="6cbff-111">notRegistered</span></span>|<span data-ttu-id="6cbff-112">0</span><span class="sxs-lookup"><span data-stu-id="6cbff-112">0</span></span>|<span data-ttu-id="6cbff-113">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="6cbff-113">The device is not registered.</span></span>|
|<span data-ttu-id="6cbff-114">注册</span><span class="sxs-lookup"><span data-stu-id="6cbff-114">registered</span></span>|<span data-ttu-id="6cbff-115">双面</span><span class="sxs-lookup"><span data-stu-id="6cbff-115">2</span></span>|<span data-ttu-id="6cbff-116">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="6cbff-116">The device is registered.</span></span>|
|<span data-ttu-id="6cbff-117">吊销</span><span class="sxs-lookup"><span data-stu-id="6cbff-117">revoked</span></span>|<span data-ttu-id="6cbff-118">第三章</span><span class="sxs-lookup"><span data-stu-id="6cbff-118">3</span></span>|<span data-ttu-id="6cbff-119">设备已被阻止、已擦除或已停用。</span><span class="sxs-lookup"><span data-stu-id="6cbff-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="6cbff-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="6cbff-120">keyConflict</span></span>|<span data-ttu-id="6cbff-121">4</span><span class="sxs-lookup"><span data-stu-id="6cbff-121">4</span></span>|<span data-ttu-id="6cbff-122">设备有键冲突。</span><span class="sxs-lookup"><span data-stu-id="6cbff-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="6cbff-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="6cbff-123">approvalPending</span></span>|<span data-ttu-id="6cbff-124">5</span><span class="sxs-lookup"><span data-stu-id="6cbff-124">5</span></span>|<span data-ttu-id="6cbff-125">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="6cbff-125">The device is pending approval.</span></span>|
|<span data-ttu-id="6cbff-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="6cbff-126">certificateReset</span></span>|<span data-ttu-id="6cbff-127">型</span><span class="sxs-lookup"><span data-stu-id="6cbff-127">6</span></span>|<span data-ttu-id="6cbff-128">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="6cbff-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="6cbff-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="6cbff-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="6cbff-130">步</span><span class="sxs-lookup"><span data-stu-id="6cbff-130">7</span></span>|<span data-ttu-id="6cbff-131">设备未注册且未完成注册。</span><span class="sxs-lookup"><span data-stu-id="6cbff-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="6cbff-132">unknown</span><span class="sxs-lookup"><span data-stu-id="6cbff-132">unknown</span></span>|<span data-ttu-id="6cbff-133">utf-8</span><span class="sxs-lookup"><span data-stu-id="6cbff-133">8</span></span>|<span data-ttu-id="6cbff-134">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="6cbff-134">The device registration status is unknown.</span></span>|





