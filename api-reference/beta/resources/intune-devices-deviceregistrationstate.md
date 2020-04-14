---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fb7e522159df19040fcc4da3870e76b7971c95c0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470676"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="d69dc-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d69dc-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="d69dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d69dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d69dc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d69dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d69dc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d69dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d69dc-107">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="d69dc-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="d69dc-108">成员</span><span class="sxs-lookup"><span data-stu-id="d69dc-108">Members</span></span>
|<span data-ttu-id="d69dc-109">成员</span><span class="sxs-lookup"><span data-stu-id="d69dc-109">Member</span></span>|<span data-ttu-id="d69dc-110">值</span><span class="sxs-lookup"><span data-stu-id="d69dc-110">Value</span></span>|<span data-ttu-id="d69dc-111">说明</span><span class="sxs-lookup"><span data-stu-id="d69dc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d69dc-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="d69dc-112">notRegistered</span></span>|<span data-ttu-id="d69dc-113">0</span><span class="sxs-lookup"><span data-stu-id="d69dc-113">0</span></span>|<span data-ttu-id="d69dc-114">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="d69dc-114">The device is not registered.</span></span>|
|<span data-ttu-id="d69dc-115">注册</span><span class="sxs-lookup"><span data-stu-id="d69dc-115">registered</span></span>|<span data-ttu-id="d69dc-116">双面</span><span class="sxs-lookup"><span data-stu-id="d69dc-116">2</span></span>|<span data-ttu-id="d69dc-117">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="d69dc-117">The device is registered.</span></span>|
|<span data-ttu-id="d69dc-118">吊销</span><span class="sxs-lookup"><span data-stu-id="d69dc-118">revoked</span></span>|<span data-ttu-id="d69dc-119">第三章</span><span class="sxs-lookup"><span data-stu-id="d69dc-119">3</span></span>|<span data-ttu-id="d69dc-120">设备已被阻止、已擦除或已停用。</span><span class="sxs-lookup"><span data-stu-id="d69dc-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="d69dc-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="d69dc-121">keyConflict</span></span>|<span data-ttu-id="d69dc-122">4 </span><span class="sxs-lookup"><span data-stu-id="d69dc-122">4</span></span>|<span data-ttu-id="d69dc-123">设备有键冲突。</span><span class="sxs-lookup"><span data-stu-id="d69dc-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="d69dc-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="d69dc-124">approvalPending</span></span>|<span data-ttu-id="d69dc-125">5 </span><span class="sxs-lookup"><span data-stu-id="d69dc-125">5</span></span>|<span data-ttu-id="d69dc-126">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="d69dc-126">The device is pending approval.</span></span>|
|<span data-ttu-id="d69dc-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="d69dc-127">certificateReset</span></span>|<span data-ttu-id="d69dc-128">6 </span><span class="sxs-lookup"><span data-stu-id="d69dc-128">6</span></span>|<span data-ttu-id="d69dc-129">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="d69dc-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="d69dc-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="d69dc-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="d69dc-131">7 </span><span class="sxs-lookup"><span data-stu-id="d69dc-131">7</span></span>|<span data-ttu-id="d69dc-132">设备未注册且未完成注册。</span><span class="sxs-lookup"><span data-stu-id="d69dc-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="d69dc-133">unknown</span><span class="sxs-lookup"><span data-stu-id="d69dc-133">unknown</span></span>|<span data-ttu-id="d69dc-134">8 </span><span class="sxs-lookup"><span data-stu-id="d69dc-134">8</span></span>|<span data-ttu-id="d69dc-135">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="d69dc-135">The device registration status is unknown.</span></span>|



