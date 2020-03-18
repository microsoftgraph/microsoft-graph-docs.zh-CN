---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 908f38a2da8f5960eb9c5f1879b7b54374b806ed
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784131"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="13a79-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="13a79-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="13a79-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13a79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13a79-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13a79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13a79-106">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="13a79-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="13a79-107">成员</span><span class="sxs-lookup"><span data-stu-id="13a79-107">Members</span></span>
|<span data-ttu-id="13a79-108">成员</span><span class="sxs-lookup"><span data-stu-id="13a79-108">Member</span></span>|<span data-ttu-id="13a79-109">值</span><span class="sxs-lookup"><span data-stu-id="13a79-109">Value</span></span>|<span data-ttu-id="13a79-110">说明</span><span class="sxs-lookup"><span data-stu-id="13a79-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13a79-111">notRegistered</span><span class="sxs-lookup"><span data-stu-id="13a79-111">notRegistered</span></span>|<span data-ttu-id="13a79-112">0</span><span class="sxs-lookup"><span data-stu-id="13a79-112">0</span></span>|<span data-ttu-id="13a79-113">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="13a79-113">The device is not registered.</span></span>|
|<span data-ttu-id="13a79-114">注册</span><span class="sxs-lookup"><span data-stu-id="13a79-114">registered</span></span>|<span data-ttu-id="13a79-115">双面</span><span class="sxs-lookup"><span data-stu-id="13a79-115">2</span></span>|<span data-ttu-id="13a79-116">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="13a79-116">The device is registered.</span></span>|
|<span data-ttu-id="13a79-117">吊销</span><span class="sxs-lookup"><span data-stu-id="13a79-117">revoked</span></span>|<span data-ttu-id="13a79-118">第三章</span><span class="sxs-lookup"><span data-stu-id="13a79-118">3</span></span>|<span data-ttu-id="13a79-119">设备已被阻止、已擦除或已停用。</span><span class="sxs-lookup"><span data-stu-id="13a79-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="13a79-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="13a79-120">keyConflict</span></span>|<span data-ttu-id="13a79-121">4 </span><span class="sxs-lookup"><span data-stu-id="13a79-121">4</span></span>|<span data-ttu-id="13a79-122">设备有键冲突。</span><span class="sxs-lookup"><span data-stu-id="13a79-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="13a79-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="13a79-123">approvalPending</span></span>|<span data-ttu-id="13a79-124">5 </span><span class="sxs-lookup"><span data-stu-id="13a79-124">5</span></span>|<span data-ttu-id="13a79-125">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="13a79-125">The device is pending approval.</span></span>|
|<span data-ttu-id="13a79-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="13a79-126">certificateReset</span></span>|<span data-ttu-id="13a79-127">6 </span><span class="sxs-lookup"><span data-stu-id="13a79-127">6</span></span>|<span data-ttu-id="13a79-128">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="13a79-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="13a79-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="13a79-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="13a79-130">7 </span><span class="sxs-lookup"><span data-stu-id="13a79-130">7</span></span>|<span data-ttu-id="13a79-131">设备未注册且未完成注册。</span><span class="sxs-lookup"><span data-stu-id="13a79-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="13a79-132">unknown</span><span class="sxs-lookup"><span data-stu-id="13a79-132">unknown</span></span>|<span data-ttu-id="13a79-133">8 </span><span class="sxs-lookup"><span data-stu-id="13a79-133">8</span></span>|<span data-ttu-id="13a79-134">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="13a79-134">The device registration status is unknown.</span></span>|



