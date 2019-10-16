---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略需要密码类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a94dabb436ec11dd340c15afcbd7ed2f04ddbca
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538635"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="008e4-103">androidDeviceOwnerRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="008e4-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="008e4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="008e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="008e4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="008e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="008e4-106">Android 设备所有者策略需要密码类型。</span><span class="sxs-lookup"><span data-stu-id="008e4-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="008e4-107">成员</span><span class="sxs-lookup"><span data-stu-id="008e4-107">Members</span></span>
|<span data-ttu-id="008e4-108">成员</span><span class="sxs-lookup"><span data-stu-id="008e4-108">Member</span></span>|<span data-ttu-id="008e4-109">值</span><span class="sxs-lookup"><span data-stu-id="008e4-109">Value</span></span>|<span data-ttu-id="008e4-110">说明</span><span class="sxs-lookup"><span data-stu-id="008e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="008e4-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="008e4-111">deviceDefault</span></span>|<span data-ttu-id="008e4-112">0</span><span class="sxs-lookup"><span data-stu-id="008e4-112">0</span></span>|<span data-ttu-id="008e4-113">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="008e4-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="008e4-114">必需</span><span class="sxs-lookup"><span data-stu-id="008e4-114">required</span></span>|<span data-ttu-id="008e4-115">1</span><span class="sxs-lookup"><span data-stu-id="008e4-115">1</span></span>|<span data-ttu-id="008e4-116">必须设置密码，但类型没有限制。</span><span class="sxs-lookup"><span data-stu-id="008e4-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="008e4-117">位数</span><span class="sxs-lookup"><span data-stu-id="008e4-117">numeric</span></span>|<span data-ttu-id="008e4-118">双面</span><span class="sxs-lookup"><span data-stu-id="008e4-118">2</span></span>|<span data-ttu-id="008e4-119">至少为数值。</span><span class="sxs-lookup"><span data-stu-id="008e4-119">At least numeric.</span></span>|
|<span data-ttu-id="008e4-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="008e4-120">numericComplex</span></span>|<span data-ttu-id="008e4-121">第三章</span><span class="sxs-lookup"><span data-stu-id="008e4-121">3</span></span>|<span data-ttu-id="008e4-122">至少不带重复或有序序列的数字。</span><span class="sxs-lookup"><span data-stu-id="008e4-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="008e4-123">字母</span><span class="sxs-lookup"><span data-stu-id="008e4-123">alphabetic</span></span>|<span data-ttu-id="008e4-124">4 </span><span class="sxs-lookup"><span data-stu-id="008e4-124">4</span></span>|<span data-ttu-id="008e4-125">至少为字母密码。</span><span class="sxs-lookup"><span data-stu-id="008e4-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="008e4-126">字母数字</span><span class="sxs-lookup"><span data-stu-id="008e4-126">alphanumeric</span></span>|<span data-ttu-id="008e4-127">5 </span><span class="sxs-lookup"><span data-stu-id="008e4-127">5</span></span>|<span data-ttu-id="008e4-128">至少为字母数字密码</span><span class="sxs-lookup"><span data-stu-id="008e4-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="008e4-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="008e4-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="008e4-130">6 </span><span class="sxs-lookup"><span data-stu-id="008e4-130">6</span></span>|<span data-ttu-id="008e4-131">至少带有符号的字母数字。</span><span class="sxs-lookup"><span data-stu-id="008e4-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="008e4-132">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="008e4-132">lowSecurityBiometric</span></span>|<span data-ttu-id="008e4-133">7 </span><span class="sxs-lookup"><span data-stu-id="008e4-133">7</span></span>|<span data-ttu-id="008e4-134">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="008e4-134">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="008e4-135">customPassword</span><span class="sxs-lookup"><span data-stu-id="008e4-135">customPassword</span></span>|<span data-ttu-id="008e4-136">8 </span><span class="sxs-lookup"><span data-stu-id="008e4-136">8</span></span>|<span data-ttu-id="008e4-137">由管理员设置的自定义密码。</span><span class="sxs-lookup"><span data-stu-id="008e4-137">Custom password set by the admin.</span></span>|



