---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5cb75fca742f1be0d4e5e00b8ba7e46da3aed954
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366781"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="77f91-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="77f91-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="77f91-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77f91-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77f91-105">Android 工作配置文件必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="77f91-105">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="77f91-106">成员</span><span class="sxs-lookup"><span data-stu-id="77f91-106">Members</span></span>
|<span data-ttu-id="77f91-107">成员</span><span class="sxs-lookup"><span data-stu-id="77f91-107">Member</span></span>|<span data-ttu-id="77f91-108">值</span><span class="sxs-lookup"><span data-stu-id="77f91-108">Value</span></span>|<span data-ttu-id="77f91-109">说明</span><span class="sxs-lookup"><span data-stu-id="77f91-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77f91-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="77f91-110">deviceDefault</span></span>|<span data-ttu-id="77f91-111">0</span><span class="sxs-lookup"><span data-stu-id="77f91-111">0</span></span>|<span data-ttu-id="77f91-112">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="77f91-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="77f91-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="77f91-113">lowSecurityBiometric</span></span>|<span data-ttu-id="77f91-114">1</span><span class="sxs-lookup"><span data-stu-id="77f91-114">1</span></span>|<span data-ttu-id="77f91-115">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="77f91-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="77f91-116">必需</span><span class="sxs-lookup"><span data-stu-id="77f91-116">required</span></span>|<span data-ttu-id="77f91-117">双面</span><span class="sxs-lookup"><span data-stu-id="77f91-117">2</span></span>|<span data-ttu-id="77f91-118">必需。</span><span class="sxs-lookup"><span data-stu-id="77f91-118">Required.</span></span>|
|<span data-ttu-id="77f91-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="77f91-119">atLeastNumeric</span></span>|<span data-ttu-id="77f91-120">第三章</span><span class="sxs-lookup"><span data-stu-id="77f91-120">3</span></span>|<span data-ttu-id="77f91-121">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="77f91-121">At least numeric password required.</span></span>|
|<span data-ttu-id="77f91-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="77f91-122">numericComplex</span></span>|<span data-ttu-id="77f91-123">4</span><span class="sxs-lookup"><span data-stu-id="77f91-123">4</span></span>|<span data-ttu-id="77f91-124">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="77f91-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="77f91-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="77f91-125">atLeastAlphabetic</span></span>|<span data-ttu-id="77f91-126">5</span><span class="sxs-lookup"><span data-stu-id="77f91-126">5</span></span>|<span data-ttu-id="77f91-127">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="77f91-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="77f91-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="77f91-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="77f91-129">型</span><span class="sxs-lookup"><span data-stu-id="77f91-129">6</span></span>|<span data-ttu-id="77f91-130">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="77f91-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="77f91-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="77f91-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="77f91-132">步</span><span class="sxs-lookup"><span data-stu-id="77f91-132">7</span></span>|<span data-ttu-id="77f91-133">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="77f91-133">At least alphanumeric with symbols password required.</span></span>|




