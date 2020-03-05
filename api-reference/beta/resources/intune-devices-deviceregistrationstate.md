---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f999e393caab410ea3f7565ade25d189193cfc40
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525024"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="c4b73-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c4b73-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="c4b73-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c4b73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4b73-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c4b73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4b73-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c4b73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4b73-107">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="c4b73-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="c4b73-108">成员</span><span class="sxs-lookup"><span data-stu-id="c4b73-108">Members</span></span>
|<span data-ttu-id="c4b73-109">成员</span><span class="sxs-lookup"><span data-stu-id="c4b73-109">Member</span></span>|<span data-ttu-id="c4b73-110">值</span><span class="sxs-lookup"><span data-stu-id="c4b73-110">Value</span></span>|<span data-ttu-id="c4b73-111">说明</span><span class="sxs-lookup"><span data-stu-id="c4b73-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4b73-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="c4b73-112">notRegistered</span></span>|<span data-ttu-id="c4b73-113">0</span><span class="sxs-lookup"><span data-stu-id="c4b73-113">0</span></span>|<span data-ttu-id="c4b73-114">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="c4b73-114">The device is not registered.</span></span>|
|<span data-ttu-id="c4b73-115">注册</span><span class="sxs-lookup"><span data-stu-id="c4b73-115">registered</span></span>|<span data-ttu-id="c4b73-116">2 </span><span class="sxs-lookup"><span data-stu-id="c4b73-116">2</span></span>|<span data-ttu-id="c4b73-117">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="c4b73-117">The device is registered.</span></span>|
|<span data-ttu-id="c4b73-118">吊销</span><span class="sxs-lookup"><span data-stu-id="c4b73-118">revoked</span></span>|<span data-ttu-id="c4b73-119">3 </span><span class="sxs-lookup"><span data-stu-id="c4b73-119">3</span></span>|<span data-ttu-id="c4b73-120">设备已被阻止、已擦除或已停用。</span><span class="sxs-lookup"><span data-stu-id="c4b73-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="c4b73-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="c4b73-121">keyConflict</span></span>|<span data-ttu-id="c4b73-122">4 </span><span class="sxs-lookup"><span data-stu-id="c4b73-122">4</span></span>|<span data-ttu-id="c4b73-123">设备有键冲突。</span><span class="sxs-lookup"><span data-stu-id="c4b73-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="c4b73-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="c4b73-124">approvalPending</span></span>|<span data-ttu-id="c4b73-125">5 </span><span class="sxs-lookup"><span data-stu-id="c4b73-125">5</span></span>|<span data-ttu-id="c4b73-126">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="c4b73-126">The device is pending approval.</span></span>|
|<span data-ttu-id="c4b73-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="c4b73-127">certificateReset</span></span>|<span data-ttu-id="c4b73-128">6 </span><span class="sxs-lookup"><span data-stu-id="c4b73-128">6</span></span>|<span data-ttu-id="c4b73-129">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="c4b73-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="c4b73-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="c4b73-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="c4b73-131">7 </span><span class="sxs-lookup"><span data-stu-id="c4b73-131">7</span></span>|<span data-ttu-id="c4b73-132">设备未注册且未完成注册。</span><span class="sxs-lookup"><span data-stu-id="c4b73-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="c4b73-133">unknown</span><span class="sxs-lookup"><span data-stu-id="c4b73-133">unknown</span></span>|<span data-ttu-id="c4b73-134">8 </span><span class="sxs-lookup"><span data-stu-id="c4b73-134">8</span></span>|<span data-ttu-id="c4b73-135">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="c4b73-135">The device registration status is unknown.</span></span>|



