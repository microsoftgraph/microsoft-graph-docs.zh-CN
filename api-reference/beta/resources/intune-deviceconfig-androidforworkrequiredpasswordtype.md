---
title: androidForWorkRequiredPasswordType 枚举类型
description: 适用于工作所需密码类型的 Android。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0026d4842785ada7a26ba97147a7d8cfeed3f0e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42484524"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="743d1-103">androidForWorkRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="743d1-103">androidForWorkRequiredPasswordType enum type</span></span>

<span data-ttu-id="743d1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="743d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="743d1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="743d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="743d1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="743d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="743d1-107">适用于工作所需密码类型的 Android。</span><span class="sxs-lookup"><span data-stu-id="743d1-107">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="743d1-108">成员</span><span class="sxs-lookup"><span data-stu-id="743d1-108">Members</span></span>
|<span data-ttu-id="743d1-109">成员</span><span class="sxs-lookup"><span data-stu-id="743d1-109">Member</span></span>|<span data-ttu-id="743d1-110">值</span><span class="sxs-lookup"><span data-stu-id="743d1-110">Value</span></span>|<span data-ttu-id="743d1-111">说明</span><span class="sxs-lookup"><span data-stu-id="743d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="743d1-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="743d1-112">deviceDefault</span></span>|<span data-ttu-id="743d1-113">0</span><span class="sxs-lookup"><span data-stu-id="743d1-113">0</span></span>|<span data-ttu-id="743d1-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="743d1-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="743d1-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="743d1-115">lowSecurityBiometric</span></span>|<span data-ttu-id="743d1-116">1 </span><span class="sxs-lookup"><span data-stu-id="743d1-116">1</span></span>|<span data-ttu-id="743d1-117">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="743d1-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="743d1-118">必需</span><span class="sxs-lookup"><span data-stu-id="743d1-118">required</span></span>|<span data-ttu-id="743d1-119">2 </span><span class="sxs-lookup"><span data-stu-id="743d1-119">2</span></span>|<span data-ttu-id="743d1-120">必填。</span><span class="sxs-lookup"><span data-stu-id="743d1-120">Required.</span></span>|
|<span data-ttu-id="743d1-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="743d1-121">atLeastNumeric</span></span>|<span data-ttu-id="743d1-122">3 </span><span class="sxs-lookup"><span data-stu-id="743d1-122">3</span></span>|<span data-ttu-id="743d1-123">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="743d1-123">At least numeric password required.</span></span>|
|<span data-ttu-id="743d1-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="743d1-124">numericComplex</span></span>|<span data-ttu-id="743d1-125">4 </span><span class="sxs-lookup"><span data-stu-id="743d1-125">4</span></span>|<span data-ttu-id="743d1-126">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="743d1-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="743d1-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="743d1-127">atLeastAlphabetic</span></span>|<span data-ttu-id="743d1-128">5 </span><span class="sxs-lookup"><span data-stu-id="743d1-128">5</span></span>|<span data-ttu-id="743d1-129">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="743d1-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="743d1-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="743d1-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="743d1-131">6 </span><span class="sxs-lookup"><span data-stu-id="743d1-131">6</span></span>|<span data-ttu-id="743d1-132">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="743d1-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="743d1-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="743d1-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="743d1-134">7 </span><span class="sxs-lookup"><span data-stu-id="743d1-134">7</span></span>|<span data-ttu-id="743d1-135">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="743d1-135">At least alphanumeric with symbols password required.</span></span>|



