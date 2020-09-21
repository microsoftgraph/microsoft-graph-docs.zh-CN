---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略需要密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d3df49d6ed508a8d9860c0bb37a234c9fd6e5c2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968694"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="9b4bb-103">androidDeviceOwnerRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9b4bb-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

<span data-ttu-id="9b4bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b4bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b4bb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b4bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b4bb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b4bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b4bb-107">Android 设备所有者策略需要密码类型。</span><span class="sxs-lookup"><span data-stu-id="9b4bb-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="9b4bb-108">成员</span><span class="sxs-lookup"><span data-stu-id="9b4bb-108">Members</span></span>
|<span data-ttu-id="9b4bb-109">成员</span><span class="sxs-lookup"><span data-stu-id="9b4bb-109">Member</span></span>|<span data-ttu-id="9b4bb-110">值</span><span class="sxs-lookup"><span data-stu-id="9b4bb-110">Value</span></span>|<span data-ttu-id="9b4bb-111">说明</span><span class="sxs-lookup"><span data-stu-id="9b4bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b4bb-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9b4bb-112">deviceDefault</span></span>|<span data-ttu-id="9b4bb-113">0</span><span class="sxs-lookup"><span data-stu-id="9b4bb-113">0</span></span>|<span data-ttu-id="9b4bb-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="9b4bb-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="9b4bb-115">必需</span><span class="sxs-lookup"><span data-stu-id="9b4bb-115">required</span></span>|<span data-ttu-id="9b4bb-116">1 </span><span class="sxs-lookup"><span data-stu-id="9b4bb-116">1</span></span>|<span data-ttu-id="9b4bb-117">必须设置密码，但类型没有限制。</span><span class="sxs-lookup"><span data-stu-id="9b4bb-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="9b4bb-118">位数</span><span class="sxs-lookup"><span data-stu-id="9b4bb-118">numeric</span></span>|<span data-ttu-id="9b4bb-119">2 </span><span class="sxs-lookup"><span data-stu-id="9b4bb-119">2</span></span>|<span data-ttu-id="9b4bb-120">至少为数值。</span><span class="sxs-lookup"><span data-stu-id="9b4bb-120">At least numeric.</span></span>|
|<span data-ttu-id="9b4bb-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="9b4bb-121">numericComplex</span></span>|<span data-ttu-id="9b4bb-122">第三章</span><span class="sxs-lookup"><span data-stu-id="9b4bb-122">3</span></span>|<span data-ttu-id="9b4bb-123">至少不带重复或有序序列的数字。</span><span class="sxs-lookup"><span data-stu-id="9b4bb-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="9b4bb-124">字母</span><span class="sxs-lookup"><span data-stu-id="9b4bb-124">alphabetic</span></span>|<span data-ttu-id="9b4bb-125">4 </span><span class="sxs-lookup"><span data-stu-id="9b4bb-125">4</span></span>|<span data-ttu-id="9b4bb-126">至少为字母密码。</span><span class="sxs-lookup"><span data-stu-id="9b4bb-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="9b4bb-127">字母数字</span><span class="sxs-lookup"><span data-stu-id="9b4bb-127">alphanumeric</span></span>|<span data-ttu-id="9b4bb-128">5 </span><span class="sxs-lookup"><span data-stu-id="9b4bb-128">5</span></span>|<span data-ttu-id="9b4bb-129">至少为字母数字密码</span><span class="sxs-lookup"><span data-stu-id="9b4bb-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="9b4bb-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="9b4bb-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="9b4bb-131">6 </span><span class="sxs-lookup"><span data-stu-id="9b4bb-131">6</span></span>|<span data-ttu-id="9b4bb-132">至少带有符号的字母数字。</span><span class="sxs-lookup"><span data-stu-id="9b4bb-132">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="9b4bb-133">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="9b4bb-133">lowSecurityBiometric</span></span>|<span data-ttu-id="9b4bb-134">7 </span><span class="sxs-lookup"><span data-stu-id="9b4bb-134">7</span></span>|<span data-ttu-id="9b4bb-135">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="9b4bb-135">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="9b4bb-136">customPassword</span><span class="sxs-lookup"><span data-stu-id="9b4bb-136">customPassword</span></span>|<span data-ttu-id="9b4bb-137">8 </span><span class="sxs-lookup"><span data-stu-id="9b4bb-137">8</span></span>|<span data-ttu-id="9b4bb-138">由管理员设置的自定义密码。</span><span class="sxs-lookup"><span data-stu-id="9b4bb-138">Custom password set by the admin.</span></span>|






