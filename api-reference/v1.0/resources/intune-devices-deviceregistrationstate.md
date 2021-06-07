---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 39a4c68f2a688564284fc6045f61b84e72b748ab
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751690"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="d3c69-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d3c69-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="d3c69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3c69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3c69-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3c69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3c69-106">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="d3c69-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="d3c69-107">成员</span><span class="sxs-lookup"><span data-stu-id="d3c69-107">Members</span></span>
|<span data-ttu-id="d3c69-108">成员</span><span class="sxs-lookup"><span data-stu-id="d3c69-108">Member</span></span>|<span data-ttu-id="d3c69-109">值</span><span class="sxs-lookup"><span data-stu-id="d3c69-109">Value</span></span>|<span data-ttu-id="d3c69-110">Description</span><span class="sxs-lookup"><span data-stu-id="d3c69-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3c69-111">notRegistered</span><span class="sxs-lookup"><span data-stu-id="d3c69-111">notRegistered</span></span>|<span data-ttu-id="d3c69-112">0</span><span class="sxs-lookup"><span data-stu-id="d3c69-112">0</span></span>|<span data-ttu-id="d3c69-113">设备未注册。</span><span class="sxs-lookup"><span data-stu-id="d3c69-113">The device is not registered.</span></span>|
|<span data-ttu-id="d3c69-114">registered</span><span class="sxs-lookup"><span data-stu-id="d3c69-114">registered</span></span>|<span data-ttu-id="d3c69-115">2</span><span class="sxs-lookup"><span data-stu-id="d3c69-115">2</span></span>|<span data-ttu-id="d3c69-116">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="d3c69-116">The device is registered.</span></span>|
|<span data-ttu-id="d3c69-117">revoked</span><span class="sxs-lookup"><span data-stu-id="d3c69-117">revoked</span></span>|<span data-ttu-id="d3c69-118">3</span><span class="sxs-lookup"><span data-stu-id="d3c69-118">3</span></span>|<span data-ttu-id="d3c69-119">设备已被阻止、擦除或停用。</span><span class="sxs-lookup"><span data-stu-id="d3c69-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="d3c69-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="d3c69-120">keyConflict</span></span>|<span data-ttu-id="d3c69-121">4 </span><span class="sxs-lookup"><span data-stu-id="d3c69-121">4</span></span>|<span data-ttu-id="d3c69-122">设备存在密钥冲突。</span><span class="sxs-lookup"><span data-stu-id="d3c69-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="d3c69-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="d3c69-123">approvalPending</span></span>|<span data-ttu-id="d3c69-124">5 </span><span class="sxs-lookup"><span data-stu-id="d3c69-124">5</span></span>|<span data-ttu-id="d3c69-125">设备正在等待审批。</span><span class="sxs-lookup"><span data-stu-id="d3c69-125">The device is pending approval.</span></span>|
|<span data-ttu-id="d3c69-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="d3c69-126">certificateReset</span></span>|<span data-ttu-id="d3c69-127">6 </span><span class="sxs-lookup"><span data-stu-id="d3c69-127">6</span></span>|<span data-ttu-id="d3c69-128">设备证书已重置。</span><span class="sxs-lookup"><span data-stu-id="d3c69-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="d3c69-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="d3c69-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="d3c69-130">7 </span><span class="sxs-lookup"><span data-stu-id="d3c69-130">7</span></span>|<span data-ttu-id="d3c69-131">设备未注册，正在等待注册。</span><span class="sxs-lookup"><span data-stu-id="d3c69-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="d3c69-132">unknown</span><span class="sxs-lookup"><span data-stu-id="d3c69-132">unknown</span></span>|<span data-ttu-id="d3c69-133">8 </span><span class="sxs-lookup"><span data-stu-id="d3c69-133">8</span></span>|<span data-ttu-id="d3c69-134">设备注册状态未知。</span><span class="sxs-lookup"><span data-stu-id="d3c69-134">The device registration status is unknown.</span></span>|




