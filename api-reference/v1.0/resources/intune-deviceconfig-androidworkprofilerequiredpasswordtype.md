---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2e9c65138a6dee7082b85261fd62c0fe9a9fd5e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028675"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="f6141-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f6141-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="f6141-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6141-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6141-105">Android 工作配置文件必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="f6141-105">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="f6141-106">成员</span><span class="sxs-lookup"><span data-stu-id="f6141-106">Members</span></span>
|<span data-ttu-id="f6141-107">成员</span><span class="sxs-lookup"><span data-stu-id="f6141-107">Member</span></span>|<span data-ttu-id="f6141-108">值</span><span class="sxs-lookup"><span data-stu-id="f6141-108">Value</span></span>|<span data-ttu-id="f6141-109">说明</span><span class="sxs-lookup"><span data-stu-id="f6141-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6141-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f6141-110">deviceDefault</span></span>|<span data-ttu-id="f6141-111">0</span><span class="sxs-lookup"><span data-stu-id="f6141-111">0</span></span>|<span data-ttu-id="f6141-112">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="f6141-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="f6141-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="f6141-113">lowSecurityBiometric</span></span>|<span data-ttu-id="f6141-114">1</span><span class="sxs-lookup"><span data-stu-id="f6141-114">1</span></span>|<span data-ttu-id="f6141-115">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="f6141-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="f6141-116">必需</span><span class="sxs-lookup"><span data-stu-id="f6141-116">required</span></span>|<span data-ttu-id="f6141-117">双面</span><span class="sxs-lookup"><span data-stu-id="f6141-117">2</span></span>|<span data-ttu-id="f6141-118">必需。</span><span class="sxs-lookup"><span data-stu-id="f6141-118">Required.</span></span>|
|<span data-ttu-id="f6141-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="f6141-119">atLeastNumeric</span></span>|<span data-ttu-id="f6141-120">第三章</span><span class="sxs-lookup"><span data-stu-id="f6141-120">3</span></span>|<span data-ttu-id="f6141-121">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="f6141-121">At least numeric password required.</span></span>|
|<span data-ttu-id="f6141-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="f6141-122">numericComplex</span></span>|<span data-ttu-id="f6141-123">4</span><span class="sxs-lookup"><span data-stu-id="f6141-123">4</span></span>|<span data-ttu-id="f6141-124">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="f6141-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="f6141-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="f6141-125">atLeastAlphabetic</span></span>|<span data-ttu-id="f6141-126">5</span><span class="sxs-lookup"><span data-stu-id="f6141-126">5</span></span>|<span data-ttu-id="f6141-127">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="f6141-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="f6141-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="f6141-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="f6141-129">型</span><span class="sxs-lookup"><span data-stu-id="f6141-129">6</span></span>|<span data-ttu-id="f6141-130">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="f6141-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="f6141-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="f6141-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="f6141-132">步</span><span class="sxs-lookup"><span data-stu-id="f6141-132">7</span></span>|<span data-ttu-id="f6141-133">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="f6141-133">At least alphanumeric with symbols password required.</span></span>|



