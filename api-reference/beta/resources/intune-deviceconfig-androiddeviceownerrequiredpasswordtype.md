---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略需要密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 376e33edac921f6771d76a45622a58bca3076c5c
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572332"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="4f15f-103">androidDeviceOwnerRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4f15f-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="4f15f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f15f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f15f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f15f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f15f-106">Android 设备所有者策略需要密码类型。</span><span class="sxs-lookup"><span data-stu-id="4f15f-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="4f15f-107">成员</span><span class="sxs-lookup"><span data-stu-id="4f15f-107">Members</span></span>
|<span data-ttu-id="4f15f-108">成员</span><span class="sxs-lookup"><span data-stu-id="4f15f-108">Member</span></span>|<span data-ttu-id="4f15f-109">值</span><span class="sxs-lookup"><span data-stu-id="4f15f-109">Value</span></span>|<span data-ttu-id="4f15f-110">说明</span><span class="sxs-lookup"><span data-stu-id="4f15f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f15f-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4f15f-111">deviceDefault</span></span>|<span data-ttu-id="4f15f-112">0</span><span class="sxs-lookup"><span data-stu-id="4f15f-112">0</span></span>|<span data-ttu-id="4f15f-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="4f15f-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="4f15f-114">必需</span><span class="sxs-lookup"><span data-stu-id="4f15f-114">required</span></span>|<span data-ttu-id="4f15f-115">1</span><span class="sxs-lookup"><span data-stu-id="4f15f-115">1</span></span>|<span data-ttu-id="4f15f-116">必须设置密码, 但类型没有限制。</span><span class="sxs-lookup"><span data-stu-id="4f15f-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="4f15f-117">位数</span><span class="sxs-lookup"><span data-stu-id="4f15f-117">numeric</span></span>|<span data-ttu-id="4f15f-118">双面</span><span class="sxs-lookup"><span data-stu-id="4f15f-118">2</span></span>|<span data-ttu-id="4f15f-119">至少为数值。</span><span class="sxs-lookup"><span data-stu-id="4f15f-119">At least numeric.</span></span>|
|<span data-ttu-id="4f15f-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="4f15f-120">numericComplex</span></span>|<span data-ttu-id="4f15f-121">第三章</span><span class="sxs-lookup"><span data-stu-id="4f15f-121">3</span></span>|<span data-ttu-id="4f15f-122">至少不带重复或有序序列的数字。</span><span class="sxs-lookup"><span data-stu-id="4f15f-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="4f15f-123">字母</span><span class="sxs-lookup"><span data-stu-id="4f15f-123">alphabetic</span></span>|<span data-ttu-id="4f15f-124">4</span><span class="sxs-lookup"><span data-stu-id="4f15f-124">4</span></span>|<span data-ttu-id="4f15f-125">至少为字母密码。</span><span class="sxs-lookup"><span data-stu-id="4f15f-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="4f15f-126">字母数字</span><span class="sxs-lookup"><span data-stu-id="4f15f-126">alphanumeric</span></span>|<span data-ttu-id="4f15f-127">5</span><span class="sxs-lookup"><span data-stu-id="4f15f-127">5</span></span>|<span data-ttu-id="4f15f-128">至少为字母数字密码</span><span class="sxs-lookup"><span data-stu-id="4f15f-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="4f15f-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="4f15f-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="4f15f-130">型</span><span class="sxs-lookup"><span data-stu-id="4f15f-130">6</span></span>|<span data-ttu-id="4f15f-131">至少带有符号的字母数字。</span><span class="sxs-lookup"><span data-stu-id="4f15f-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="4f15f-132">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="4f15f-132">lowSecurityBiometric</span></span>|<span data-ttu-id="4f15f-133">步</span><span class="sxs-lookup"><span data-stu-id="4f15f-133">7</span></span>|<span data-ttu-id="4f15f-134">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="4f15f-134">Low security biometrics based password required.</span></span>|




