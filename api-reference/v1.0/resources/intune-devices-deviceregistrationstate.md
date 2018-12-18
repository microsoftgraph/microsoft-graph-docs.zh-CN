---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: tfitzmac
ms.openlocfilehash: 9fdd5cd3a63472e841f0d97f8cbee3a0f548380d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320088"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="42254-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="42254-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="42254-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="42254-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42254-105">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="42254-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="42254-106">成员</span><span class="sxs-lookup"><span data-stu-id="42254-106">Members</span></span>
|<span data-ttu-id="42254-107">成员</span><span class="sxs-lookup"><span data-stu-id="42254-107">Member</span></span>|<span data-ttu-id="42254-108">值</span><span class="sxs-lookup"><span data-stu-id="42254-108">Value</span></span>|<span data-ttu-id="42254-109">说明</span><span class="sxs-lookup"><span data-stu-id="42254-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42254-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="42254-110">notRegistered</span></span>|<span data-ttu-id="42254-111">0</span><span class="sxs-lookup"><span data-stu-id="42254-111">0</span></span>|<span data-ttu-id="42254-112">未注册设备。</span><span class="sxs-lookup"><span data-stu-id="42254-112">The device is not registered.</span></span>|
|<span data-ttu-id="42254-113">注册</span><span class="sxs-lookup"><span data-stu-id="42254-113">registered</span></span>|<span data-ttu-id="42254-114">2</span><span class="sxs-lookup"><span data-stu-id="42254-114">2</span></span>|<span data-ttu-id="42254-115">已注册设备。</span><span class="sxs-lookup"><span data-stu-id="42254-115">The device is registered.</span></span>|
|<span data-ttu-id="42254-116">吊销</span><span class="sxs-lookup"><span data-stu-id="42254-116">revoked</span></span>|<span data-ttu-id="42254-117">3</span><span class="sxs-lookup"><span data-stu-id="42254-117">3</span></span>|<span data-ttu-id="42254-118">已阻止、 擦除或停用该设备。</span><span class="sxs-lookup"><span data-stu-id="42254-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="42254-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="42254-119">keyConflict</span></span>|<span data-ttu-id="42254-120">4</span><span class="sxs-lookup"><span data-stu-id="42254-120">4</span></span>|<span data-ttu-id="42254-121">设备具有键冲突。</span><span class="sxs-lookup"><span data-stu-id="42254-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="42254-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="42254-122">approvalPending</span></span>|<span data-ttu-id="42254-123">5</span><span class="sxs-lookup"><span data-stu-id="42254-123">5</span></span>|<span data-ttu-id="42254-124">设备是待审批状态。</span><span class="sxs-lookup"><span data-stu-id="42254-124">The device is pending approval.</span></span>|
|<span data-ttu-id="42254-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="42254-125">certificateReset</span></span>|<span data-ttu-id="42254-126">6</span><span class="sxs-lookup"><span data-stu-id="42254-126">6</span></span>|<span data-ttu-id="42254-127">设备证书已被重置。</span><span class="sxs-lookup"><span data-stu-id="42254-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="42254-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="42254-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="42254-129">7</span><span class="sxs-lookup"><span data-stu-id="42254-129">7</span></span>|<span data-ttu-id="42254-130">未注册设备以及待处理的注册。</span><span class="sxs-lookup"><span data-stu-id="42254-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="42254-131">unknown</span><span class="sxs-lookup"><span data-stu-id="42254-131">unknown</span></span>|<span data-ttu-id="42254-132">8</span><span class="sxs-lookup"><span data-stu-id="42254-132">8</span></span>|<span data-ttu-id="42254-133">未知设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="42254-133">The device registration status is unknown.</span></span>|



