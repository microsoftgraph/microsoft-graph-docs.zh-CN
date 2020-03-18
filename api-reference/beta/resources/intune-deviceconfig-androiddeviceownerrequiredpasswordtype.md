---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略需要密码类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e6d783f8bdf5faeed2d3e10a9286a897c8d85783
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796984"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="fb761-103">androidDeviceOwnerRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fb761-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="fb761-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fb761-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb761-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb761-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb761-106">Android 设备所有者策略需要密码类型。</span><span class="sxs-lookup"><span data-stu-id="fb761-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="fb761-107">成员</span><span class="sxs-lookup"><span data-stu-id="fb761-107">Members</span></span>
|<span data-ttu-id="fb761-108">成员</span><span class="sxs-lookup"><span data-stu-id="fb761-108">Member</span></span>|<span data-ttu-id="fb761-109">值</span><span class="sxs-lookup"><span data-stu-id="fb761-109">Value</span></span>|<span data-ttu-id="fb761-110">说明</span><span class="sxs-lookup"><span data-stu-id="fb761-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb761-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="fb761-111">deviceDefault</span></span>|<span data-ttu-id="fb761-112">0</span><span class="sxs-lookup"><span data-stu-id="fb761-112">0</span></span>|<span data-ttu-id="fb761-113">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="fb761-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="fb761-114">必需</span><span class="sxs-lookup"><span data-stu-id="fb761-114">required</span></span>|<span data-ttu-id="fb761-115">1</span><span class="sxs-lookup"><span data-stu-id="fb761-115">1</span></span>|<span data-ttu-id="fb761-116">必须设置密码，但类型没有限制。</span><span class="sxs-lookup"><span data-stu-id="fb761-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="fb761-117">位数</span><span class="sxs-lookup"><span data-stu-id="fb761-117">numeric</span></span>|<span data-ttu-id="fb761-118">双面</span><span class="sxs-lookup"><span data-stu-id="fb761-118">2</span></span>|<span data-ttu-id="fb761-119">至少为数值。</span><span class="sxs-lookup"><span data-stu-id="fb761-119">At least numeric.</span></span>|
|<span data-ttu-id="fb761-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="fb761-120">numericComplex</span></span>|<span data-ttu-id="fb761-121">第三章</span><span class="sxs-lookup"><span data-stu-id="fb761-121">3</span></span>|<span data-ttu-id="fb761-122">至少不带重复或有序序列的数字。</span><span class="sxs-lookup"><span data-stu-id="fb761-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="fb761-123">字母</span><span class="sxs-lookup"><span data-stu-id="fb761-123">alphabetic</span></span>|<span data-ttu-id="fb761-124">4 </span><span class="sxs-lookup"><span data-stu-id="fb761-124">4</span></span>|<span data-ttu-id="fb761-125">至少为字母密码。</span><span class="sxs-lookup"><span data-stu-id="fb761-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="fb761-126">字母数字</span><span class="sxs-lookup"><span data-stu-id="fb761-126">alphanumeric</span></span>|<span data-ttu-id="fb761-127">5 </span><span class="sxs-lookup"><span data-stu-id="fb761-127">5</span></span>|<span data-ttu-id="fb761-128">至少为字母数字密码</span><span class="sxs-lookup"><span data-stu-id="fb761-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="fb761-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="fb761-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="fb761-130">6 </span><span class="sxs-lookup"><span data-stu-id="fb761-130">6</span></span>|<span data-ttu-id="fb761-131">至少带有符号的字母数字。</span><span class="sxs-lookup"><span data-stu-id="fb761-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="fb761-132">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="fb761-132">lowSecurityBiometric</span></span>|<span data-ttu-id="fb761-133">7 </span><span class="sxs-lookup"><span data-stu-id="fb761-133">7</span></span>|<span data-ttu-id="fb761-134">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="fb761-134">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="fb761-135">customPassword</span><span class="sxs-lookup"><span data-stu-id="fb761-135">customPassword</span></span>|<span data-ttu-id="fb761-136">8 </span><span class="sxs-lookup"><span data-stu-id="fb761-136">8</span></span>|<span data-ttu-id="fb761-137">由管理员设置的自定义密码。</span><span class="sxs-lookup"><span data-stu-id="fb761-137">Custom password set by the admin.</span></span>|



