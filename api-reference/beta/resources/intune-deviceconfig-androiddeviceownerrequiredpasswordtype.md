---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略需要密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 09714a743c441058f0a87ff9d26b864a28022b96
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707834"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="025ec-103">androidDeviceOwnerRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="025ec-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

<span data-ttu-id="025ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="025ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="025ec-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="025ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="025ec-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="025ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="025ec-107">Android 设备所有者策略需要密码类型。</span><span class="sxs-lookup"><span data-stu-id="025ec-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="025ec-108">成员</span><span class="sxs-lookup"><span data-stu-id="025ec-108">Members</span></span>
|<span data-ttu-id="025ec-109">成员</span><span class="sxs-lookup"><span data-stu-id="025ec-109">Member</span></span>|<span data-ttu-id="025ec-110">值</span><span class="sxs-lookup"><span data-stu-id="025ec-110">Value</span></span>|<span data-ttu-id="025ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="025ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="025ec-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="025ec-112">deviceDefault</span></span>|<span data-ttu-id="025ec-113">0</span><span class="sxs-lookup"><span data-stu-id="025ec-113">0</span></span>|<span data-ttu-id="025ec-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="025ec-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="025ec-115">必需</span><span class="sxs-lookup"><span data-stu-id="025ec-115">required</span></span>|<span data-ttu-id="025ec-116">1</span><span class="sxs-lookup"><span data-stu-id="025ec-116">1</span></span>|<span data-ttu-id="025ec-117">必须设置密码，但类型没有限制。</span><span class="sxs-lookup"><span data-stu-id="025ec-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="025ec-118">位数</span><span class="sxs-lookup"><span data-stu-id="025ec-118">numeric</span></span>|<span data-ttu-id="025ec-119">双面</span><span class="sxs-lookup"><span data-stu-id="025ec-119">2</span></span>|<span data-ttu-id="025ec-120">至少为数值。</span><span class="sxs-lookup"><span data-stu-id="025ec-120">At least numeric.</span></span>|
|<span data-ttu-id="025ec-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="025ec-121">numericComplex</span></span>|<span data-ttu-id="025ec-122">第三章</span><span class="sxs-lookup"><span data-stu-id="025ec-122">3</span></span>|<span data-ttu-id="025ec-123">至少不带重复或有序序列的数字。</span><span class="sxs-lookup"><span data-stu-id="025ec-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="025ec-124">字母</span><span class="sxs-lookup"><span data-stu-id="025ec-124">alphabetic</span></span>|<span data-ttu-id="025ec-125">4 </span><span class="sxs-lookup"><span data-stu-id="025ec-125">4</span></span>|<span data-ttu-id="025ec-126">至少为字母密码。</span><span class="sxs-lookup"><span data-stu-id="025ec-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="025ec-127">字母数字</span><span class="sxs-lookup"><span data-stu-id="025ec-127">alphanumeric</span></span>|<span data-ttu-id="025ec-128">5 </span><span class="sxs-lookup"><span data-stu-id="025ec-128">5</span></span>|<span data-ttu-id="025ec-129">至少为字母数字密码</span><span class="sxs-lookup"><span data-stu-id="025ec-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="025ec-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="025ec-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="025ec-131">6 </span><span class="sxs-lookup"><span data-stu-id="025ec-131">6</span></span>|<span data-ttu-id="025ec-132">至少带有符号的字母数字。</span><span class="sxs-lookup"><span data-stu-id="025ec-132">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="025ec-133">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="025ec-133">lowSecurityBiometric</span></span>|<span data-ttu-id="025ec-134">7 </span><span class="sxs-lookup"><span data-stu-id="025ec-134">7</span></span>|<span data-ttu-id="025ec-135">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="025ec-135">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="025ec-136">customPassword</span><span class="sxs-lookup"><span data-stu-id="025ec-136">customPassword</span></span>|<span data-ttu-id="025ec-137">8 </span><span class="sxs-lookup"><span data-stu-id="025ec-137">8</span></span>|<span data-ttu-id="025ec-138">由管理员设置的自定义密码。</span><span class="sxs-lookup"><span data-stu-id="025ec-138">Custom password set by the admin.</span></span>|





