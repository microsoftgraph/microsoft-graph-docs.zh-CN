---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略需要密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8c575b1b39592eb8191e358563abb6d6bd834e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556359"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="c3ba9-103">androidDeviceOwnerRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c3ba9-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="c3ba9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c3ba9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3ba9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3ba9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3ba9-106">Android 设备所有者策略需要密码类型。</span><span class="sxs-lookup"><span data-stu-id="c3ba9-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="c3ba9-107">成员</span><span class="sxs-lookup"><span data-stu-id="c3ba9-107">Members</span></span>
|<span data-ttu-id="c3ba9-108">成员</span><span class="sxs-lookup"><span data-stu-id="c3ba9-108">Member</span></span>|<span data-ttu-id="c3ba9-109">值</span><span class="sxs-lookup"><span data-stu-id="c3ba9-109">Value</span></span>|<span data-ttu-id="c3ba9-110">说明</span><span class="sxs-lookup"><span data-stu-id="c3ba9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3ba9-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c3ba9-111">deviceDefault</span></span>|<span data-ttu-id="c3ba9-112">0</span><span class="sxs-lookup"><span data-stu-id="c3ba9-112">0</span></span>|<span data-ttu-id="c3ba9-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="c3ba9-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="c3ba9-114">必需</span><span class="sxs-lookup"><span data-stu-id="c3ba9-114">required</span></span>|<span data-ttu-id="c3ba9-115">1</span><span class="sxs-lookup"><span data-stu-id="c3ba9-115">1</span></span>|<span data-ttu-id="c3ba9-116">必须设置密码, 但类型没有限制。</span><span class="sxs-lookup"><span data-stu-id="c3ba9-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="c3ba9-117">位数</span><span class="sxs-lookup"><span data-stu-id="c3ba9-117">numeric</span></span>|<span data-ttu-id="c3ba9-118">2 </span><span class="sxs-lookup"><span data-stu-id="c3ba9-118">2</span></span>|<span data-ttu-id="c3ba9-119">至少为数值。</span><span class="sxs-lookup"><span data-stu-id="c3ba9-119">At least numeric.</span></span>|
|<span data-ttu-id="c3ba9-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="c3ba9-120">numericComplex</span></span>|<span data-ttu-id="c3ba9-121">3 </span><span class="sxs-lookup"><span data-stu-id="c3ba9-121">3</span></span>|<span data-ttu-id="c3ba9-122">至少不带重复或有序序列的数字。</span><span class="sxs-lookup"><span data-stu-id="c3ba9-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="c3ba9-123">字母</span><span class="sxs-lookup"><span data-stu-id="c3ba9-123">alphabetic</span></span>|<span data-ttu-id="c3ba9-124">4 </span><span class="sxs-lookup"><span data-stu-id="c3ba9-124">4</span></span>|<span data-ttu-id="c3ba9-125">至少为字母密码。</span><span class="sxs-lookup"><span data-stu-id="c3ba9-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="c3ba9-126">字母数字</span><span class="sxs-lookup"><span data-stu-id="c3ba9-126">alphanumeric</span></span>|<span data-ttu-id="c3ba9-127">5 </span><span class="sxs-lookup"><span data-stu-id="c3ba9-127">5</span></span>|<span data-ttu-id="c3ba9-128">至少为字母数字密码</span><span class="sxs-lookup"><span data-stu-id="c3ba9-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="c3ba9-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="c3ba9-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="c3ba9-130">6 </span><span class="sxs-lookup"><span data-stu-id="c3ba9-130">6</span></span>|<span data-ttu-id="c3ba9-131">至少带有符号的字母数字。</span><span class="sxs-lookup"><span data-stu-id="c3ba9-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="c3ba9-132">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="c3ba9-132">lowSecurityBiometric</span></span>|<span data-ttu-id="c3ba9-133">7 </span><span class="sxs-lookup"><span data-stu-id="c3ba9-133">7</span></span>|<span data-ttu-id="c3ba9-134">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="c3ba9-134">Low security biometrics based password required.</span></span>|





