---
title: androidForWorkRequiredPasswordType 枚举类型
description: 适用于工作所需密码类型的 Android。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 78e9a5dc041330fb625568f5de1efeabaac3a833
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334526"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="97864-103">androidForWorkRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="97864-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="97864-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="97864-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97864-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97864-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97864-106">适用于工作所需密码类型的 Android。</span><span class="sxs-lookup"><span data-stu-id="97864-106">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="97864-107">成员</span><span class="sxs-lookup"><span data-stu-id="97864-107">Members</span></span>
|<span data-ttu-id="97864-108">成员</span><span class="sxs-lookup"><span data-stu-id="97864-108">Member</span></span>|<span data-ttu-id="97864-109">值</span><span class="sxs-lookup"><span data-stu-id="97864-109">Value</span></span>|<span data-ttu-id="97864-110">说明</span><span class="sxs-lookup"><span data-stu-id="97864-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97864-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="97864-111">deviceDefault</span></span>|<span data-ttu-id="97864-112">0</span><span class="sxs-lookup"><span data-stu-id="97864-112">0</span></span>|<span data-ttu-id="97864-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="97864-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="97864-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="97864-114">lowSecurityBiometric</span></span>|<span data-ttu-id="97864-115">1</span><span class="sxs-lookup"><span data-stu-id="97864-115">1</span></span>|<span data-ttu-id="97864-116">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="97864-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="97864-117">必需</span><span class="sxs-lookup"><span data-stu-id="97864-117">required</span></span>|<span data-ttu-id="97864-118">双面</span><span class="sxs-lookup"><span data-stu-id="97864-118">2</span></span>|<span data-ttu-id="97864-119">必需。</span><span class="sxs-lookup"><span data-stu-id="97864-119">Required.</span></span>|
|<span data-ttu-id="97864-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="97864-120">atLeastNumeric</span></span>|<span data-ttu-id="97864-121">第三章</span><span class="sxs-lookup"><span data-stu-id="97864-121">3</span></span>|<span data-ttu-id="97864-122">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="97864-122">At least numeric password required.</span></span>|
|<span data-ttu-id="97864-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="97864-123">numericComplex</span></span>|<span data-ttu-id="97864-124">4</span><span class="sxs-lookup"><span data-stu-id="97864-124">4</span></span>|<span data-ttu-id="97864-125">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="97864-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="97864-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="97864-126">atLeastAlphabetic</span></span>|<span data-ttu-id="97864-127">5</span><span class="sxs-lookup"><span data-stu-id="97864-127">5</span></span>|<span data-ttu-id="97864-128">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="97864-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="97864-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="97864-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="97864-130">型</span><span class="sxs-lookup"><span data-stu-id="97864-130">6</span></span>|<span data-ttu-id="97864-131">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="97864-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="97864-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="97864-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="97864-133">步</span><span class="sxs-lookup"><span data-stu-id="97864-133">7</span></span>|<span data-ttu-id="97864-134">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="97864-134">At least alphanumeric with symbols password required.</span></span>|



