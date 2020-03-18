---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 28b02f37bad557f71901c15d03ba963143cb05f3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796129"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="4bed5-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4bed5-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="4bed5-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4bed5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bed5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4bed5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bed5-106">Android 工作配置文件必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="4bed5-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="4bed5-107">成员</span><span class="sxs-lookup"><span data-stu-id="4bed5-107">Members</span></span>
|<span data-ttu-id="4bed5-108">成员</span><span class="sxs-lookup"><span data-stu-id="4bed5-108">Member</span></span>|<span data-ttu-id="4bed5-109">值</span><span class="sxs-lookup"><span data-stu-id="4bed5-109">Value</span></span>|<span data-ttu-id="4bed5-110">说明</span><span class="sxs-lookup"><span data-stu-id="4bed5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bed5-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4bed5-111">deviceDefault</span></span>|<span data-ttu-id="4bed5-112">0</span><span class="sxs-lookup"><span data-stu-id="4bed5-112">0</span></span>|<span data-ttu-id="4bed5-113">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="4bed5-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="4bed5-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="4bed5-114">lowSecurityBiometric</span></span>|<span data-ttu-id="4bed5-115">1</span><span class="sxs-lookup"><span data-stu-id="4bed5-115">1</span></span>|<span data-ttu-id="4bed5-116">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="4bed5-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="4bed5-117">必需</span><span class="sxs-lookup"><span data-stu-id="4bed5-117">required</span></span>|<span data-ttu-id="4bed5-118">双面</span><span class="sxs-lookup"><span data-stu-id="4bed5-118">2</span></span>|<span data-ttu-id="4bed5-119">必需。</span><span class="sxs-lookup"><span data-stu-id="4bed5-119">Required.</span></span>|
|<span data-ttu-id="4bed5-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="4bed5-120">atLeastNumeric</span></span>|<span data-ttu-id="4bed5-121">第三章</span><span class="sxs-lookup"><span data-stu-id="4bed5-121">3</span></span>|<span data-ttu-id="4bed5-122">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="4bed5-122">At least numeric password required.</span></span>|
|<span data-ttu-id="4bed5-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="4bed5-123">numericComplex</span></span>|<span data-ttu-id="4bed5-124">4 </span><span class="sxs-lookup"><span data-stu-id="4bed5-124">4</span></span>|<span data-ttu-id="4bed5-125">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="4bed5-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="4bed5-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="4bed5-126">atLeastAlphabetic</span></span>|<span data-ttu-id="4bed5-127">5 </span><span class="sxs-lookup"><span data-stu-id="4bed5-127">5</span></span>|<span data-ttu-id="4bed5-128">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="4bed5-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="4bed5-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="4bed5-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="4bed5-130">6 </span><span class="sxs-lookup"><span data-stu-id="4bed5-130">6</span></span>|<span data-ttu-id="4bed5-131">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="4bed5-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="4bed5-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="4bed5-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="4bed5-133">7 </span><span class="sxs-lookup"><span data-stu-id="4bed5-133">7</span></span>|<span data-ttu-id="4bed5-134">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="4bed5-134">At least alphanumeric with symbols password required.</span></span>|



