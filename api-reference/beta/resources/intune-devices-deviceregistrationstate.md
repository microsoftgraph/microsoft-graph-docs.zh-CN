---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 92171fb3e9fc50e516ed4568cceea03c5e0ba1cf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369932"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="025b6-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="025b6-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="025b6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="025b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="025b6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="025b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="025b6-106">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="025b6-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="025b6-107">成员</span><span class="sxs-lookup"><span data-stu-id="025b6-107">Members</span></span>
|<span data-ttu-id="025b6-108">成员</span><span class="sxs-lookup"><span data-stu-id="025b6-108">Member</span></span>|<span data-ttu-id="025b6-109">值</span><span class="sxs-lookup"><span data-stu-id="025b6-109">Value</span></span>|<span data-ttu-id="025b6-110">说明</span><span class="sxs-lookup"><span data-stu-id="025b6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="025b6-111">notRegistered</span><span class="sxs-lookup"><span data-stu-id="025b6-111">notRegistered</span></span>|<span data-ttu-id="025b6-112">0</span><span class="sxs-lookup"><span data-stu-id="025b6-112">0</span></span>|<span data-ttu-id="025b6-113">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="025b6-113">The device is not registered.</span></span>|
|<span data-ttu-id="025b6-114">注册</span><span class="sxs-lookup"><span data-stu-id="025b6-114">registered</span></span>|<span data-ttu-id="025b6-115">双面</span><span class="sxs-lookup"><span data-stu-id="025b6-115">2</span></span>|<span data-ttu-id="025b6-116">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="025b6-116">The device is registered.</span></span>|
|<span data-ttu-id="025b6-117">吊销</span><span class="sxs-lookup"><span data-stu-id="025b6-117">revoked</span></span>|<span data-ttu-id="025b6-118">第三章</span><span class="sxs-lookup"><span data-stu-id="025b6-118">3</span></span>|<span data-ttu-id="025b6-119">设备已被阻止、已擦除或已停用。</span><span class="sxs-lookup"><span data-stu-id="025b6-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="025b6-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="025b6-120">keyConflict</span></span>|<span data-ttu-id="025b6-121">4</span><span class="sxs-lookup"><span data-stu-id="025b6-121">4</span></span>|<span data-ttu-id="025b6-122">设备有键冲突。</span><span class="sxs-lookup"><span data-stu-id="025b6-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="025b6-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="025b6-123">approvalPending</span></span>|<span data-ttu-id="025b6-124">5</span><span class="sxs-lookup"><span data-stu-id="025b6-124">5</span></span>|<span data-ttu-id="025b6-125">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="025b6-125">The device is pending approval.</span></span>|
|<span data-ttu-id="025b6-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="025b6-126">certificateReset</span></span>|<span data-ttu-id="025b6-127">型</span><span class="sxs-lookup"><span data-stu-id="025b6-127">6</span></span>|<span data-ttu-id="025b6-128">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="025b6-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="025b6-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="025b6-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="025b6-130">步</span><span class="sxs-lookup"><span data-stu-id="025b6-130">7</span></span>|<span data-ttu-id="025b6-131">设备未注册且未完成注册。</span><span class="sxs-lookup"><span data-stu-id="025b6-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="025b6-132">unknown</span><span class="sxs-lookup"><span data-stu-id="025b6-132">unknown</span></span>|<span data-ttu-id="025b6-133">utf-8</span><span class="sxs-lookup"><span data-stu-id="025b6-133">8</span></span>|<span data-ttu-id="025b6-134">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="025b6-134">The device registration status is unknown.</span></span>|



