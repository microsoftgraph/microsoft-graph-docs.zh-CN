---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b384c6d5bcc3c79a967d1a4c4cdfc8299d1a56d8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947664"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="10fe3-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="10fe3-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="10fe3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10fe3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10fe3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10fe3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10fe3-106">Android 工作配置文件必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="10fe3-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="10fe3-107">成员</span><span class="sxs-lookup"><span data-stu-id="10fe3-107">Members</span></span>
|<span data-ttu-id="10fe3-108">成员</span><span class="sxs-lookup"><span data-stu-id="10fe3-108">Member</span></span>|<span data-ttu-id="10fe3-109">值</span><span class="sxs-lookup"><span data-stu-id="10fe3-109">Value</span></span>|<span data-ttu-id="10fe3-110">说明</span><span class="sxs-lookup"><span data-stu-id="10fe3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10fe3-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="10fe3-111">deviceDefault</span></span>|<span data-ttu-id="10fe3-112">0</span><span class="sxs-lookup"><span data-stu-id="10fe3-112">0</span></span>|<span data-ttu-id="10fe3-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="10fe3-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="10fe3-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="10fe3-114">lowSecurityBiometric</span></span>|<span data-ttu-id="10fe3-115">1</span><span class="sxs-lookup"><span data-stu-id="10fe3-115">1</span></span>|<span data-ttu-id="10fe3-116">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="10fe3-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="10fe3-117">必需</span><span class="sxs-lookup"><span data-stu-id="10fe3-117">required</span></span>|<span data-ttu-id="10fe3-118">双面</span><span class="sxs-lookup"><span data-stu-id="10fe3-118">2</span></span>|<span data-ttu-id="10fe3-119">必需。</span><span class="sxs-lookup"><span data-stu-id="10fe3-119">Required.</span></span>|
|<span data-ttu-id="10fe3-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="10fe3-120">atLeastNumeric</span></span>|<span data-ttu-id="10fe3-121">第三章</span><span class="sxs-lookup"><span data-stu-id="10fe3-121">3</span></span>|<span data-ttu-id="10fe3-122">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="10fe3-122">At least numeric password required.</span></span>|
|<span data-ttu-id="10fe3-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="10fe3-123">numericComplex</span></span>|<span data-ttu-id="10fe3-124">4</span><span class="sxs-lookup"><span data-stu-id="10fe3-124">4</span></span>|<span data-ttu-id="10fe3-125">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="10fe3-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="10fe3-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="10fe3-126">atLeastAlphabetic</span></span>|<span data-ttu-id="10fe3-127">5</span><span class="sxs-lookup"><span data-stu-id="10fe3-127">5</span></span>|<span data-ttu-id="10fe3-128">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="10fe3-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="10fe3-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="10fe3-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="10fe3-130">型</span><span class="sxs-lookup"><span data-stu-id="10fe3-130">6</span></span>|<span data-ttu-id="10fe3-131">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="10fe3-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="10fe3-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="10fe3-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="10fe3-133">步</span><span class="sxs-lookup"><span data-stu-id="10fe3-133">7</span></span>|<span data-ttu-id="10fe3-134">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="10fe3-134">At least alphanumeric with symbols password required.</span></span>|




