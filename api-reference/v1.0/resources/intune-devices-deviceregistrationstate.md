---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5b0048385930166de3329ef9d407f5ddd19efc77
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911894"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="3de2c-103">deviceRegistrationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3de2c-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="3de2c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3de2c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3de2c-105">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="3de2c-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="3de2c-106">成员</span><span class="sxs-lookup"><span data-stu-id="3de2c-106">Members</span></span>
|<span data-ttu-id="3de2c-107">成员</span><span class="sxs-lookup"><span data-stu-id="3de2c-107">Member</span></span>|<span data-ttu-id="3de2c-108">值</span><span class="sxs-lookup"><span data-stu-id="3de2c-108">Value</span></span>|<span data-ttu-id="3de2c-109">Description</span><span class="sxs-lookup"><span data-stu-id="3de2c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3de2c-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="3de2c-110">notRegistered</span></span>|<span data-ttu-id="3de2c-111">0</span><span class="sxs-lookup"><span data-stu-id="3de2c-111">0</span></span>|<span data-ttu-id="3de2c-112">未注册设备。</span><span class="sxs-lookup"><span data-stu-id="3de2c-112">The device is not registered.</span></span>|
|<span data-ttu-id="3de2c-113">注册</span><span class="sxs-lookup"><span data-stu-id="3de2c-113">registered</span></span>|<span data-ttu-id="3de2c-114">2</span><span class="sxs-lookup"><span data-stu-id="3de2c-114">2</span></span>|<span data-ttu-id="3de2c-115">已注册设备。</span><span class="sxs-lookup"><span data-stu-id="3de2c-115">The device is registered.</span></span>|
|<span data-ttu-id="3de2c-116">吊销</span><span class="sxs-lookup"><span data-stu-id="3de2c-116">revoked</span></span>|<span data-ttu-id="3de2c-117">3</span><span class="sxs-lookup"><span data-stu-id="3de2c-117">3</span></span>|<span data-ttu-id="3de2c-118">已阻止、 擦除或停用该设备。</span><span class="sxs-lookup"><span data-stu-id="3de2c-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="3de2c-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="3de2c-119">keyConflict</span></span>|<span data-ttu-id="3de2c-120">4</span><span class="sxs-lookup"><span data-stu-id="3de2c-120">4</span></span>|<span data-ttu-id="3de2c-121">设备具有键冲突。</span><span class="sxs-lookup"><span data-stu-id="3de2c-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="3de2c-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="3de2c-122">approvalPending</span></span>|<span data-ttu-id="3de2c-123">5</span><span class="sxs-lookup"><span data-stu-id="3de2c-123">5</span></span>|<span data-ttu-id="3de2c-124">设备是待审批状态。</span><span class="sxs-lookup"><span data-stu-id="3de2c-124">The device is pending approval.</span></span>|
|<span data-ttu-id="3de2c-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="3de2c-125">certificateReset</span></span>|<span data-ttu-id="3de2c-126">6</span><span class="sxs-lookup"><span data-stu-id="3de2c-126">6</span></span>|<span data-ttu-id="3de2c-127">设备证书已被重置。</span><span class="sxs-lookup"><span data-stu-id="3de2c-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="3de2c-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="3de2c-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="3de2c-129">7</span><span class="sxs-lookup"><span data-stu-id="3de2c-129">7</span></span>|<span data-ttu-id="3de2c-130">未注册设备以及待处理的注册。</span><span class="sxs-lookup"><span data-stu-id="3de2c-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="3de2c-131">unknown</span><span class="sxs-lookup"><span data-stu-id="3de2c-131">unknown</span></span>|<span data-ttu-id="3de2c-132">8</span><span class="sxs-lookup"><span data-stu-id="3de2c-132">8</span></span>|<span data-ttu-id="3de2c-133">未知设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="3de2c-133">The device registration status is unknown.</span></span>|



