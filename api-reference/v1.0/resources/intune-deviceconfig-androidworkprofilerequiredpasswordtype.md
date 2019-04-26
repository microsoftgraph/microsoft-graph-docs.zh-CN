---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1dbb0b7e523ea6ca3ac1be3328cf58e30d9a892
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575154"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="16bfe-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="16bfe-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="16bfe-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16bfe-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16bfe-105">Android 工作配置文件必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="16bfe-105">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="16bfe-106">成员</span><span class="sxs-lookup"><span data-stu-id="16bfe-106">Members</span></span>
|<span data-ttu-id="16bfe-107">成员</span><span class="sxs-lookup"><span data-stu-id="16bfe-107">Member</span></span>|<span data-ttu-id="16bfe-108">值</span><span class="sxs-lookup"><span data-stu-id="16bfe-108">Value</span></span>|<span data-ttu-id="16bfe-109">说明</span><span class="sxs-lookup"><span data-stu-id="16bfe-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16bfe-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="16bfe-110">deviceDefault</span></span>|<span data-ttu-id="16bfe-111">0</span><span class="sxs-lookup"><span data-stu-id="16bfe-111">0</span></span>|<span data-ttu-id="16bfe-112">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="16bfe-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="16bfe-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="16bfe-113">lowSecurityBiometric</span></span>|<span data-ttu-id="16bfe-114">1</span><span class="sxs-lookup"><span data-stu-id="16bfe-114">1</span></span>|<span data-ttu-id="16bfe-115">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="16bfe-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="16bfe-116">必需</span><span class="sxs-lookup"><span data-stu-id="16bfe-116">required</span></span>|<span data-ttu-id="16bfe-117">2 </span><span class="sxs-lookup"><span data-stu-id="16bfe-117">2</span></span>|<span data-ttu-id="16bfe-118">必需。</span><span class="sxs-lookup"><span data-stu-id="16bfe-118">Required.</span></span>|
|<span data-ttu-id="16bfe-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="16bfe-119">atLeastNumeric</span></span>|<span data-ttu-id="16bfe-120">3 </span><span class="sxs-lookup"><span data-stu-id="16bfe-120">3</span></span>|<span data-ttu-id="16bfe-121">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="16bfe-121">At least numeric password required.</span></span>|
|<span data-ttu-id="16bfe-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="16bfe-122">numericComplex</span></span>|<span data-ttu-id="16bfe-123">4 </span><span class="sxs-lookup"><span data-stu-id="16bfe-123">4</span></span>|<span data-ttu-id="16bfe-124">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="16bfe-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="16bfe-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="16bfe-125">atLeastAlphabetic</span></span>|<span data-ttu-id="16bfe-126">5 </span><span class="sxs-lookup"><span data-stu-id="16bfe-126">5</span></span>|<span data-ttu-id="16bfe-127">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="16bfe-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="16bfe-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="16bfe-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="16bfe-129">6 </span><span class="sxs-lookup"><span data-stu-id="16bfe-129">6</span></span>|<span data-ttu-id="16bfe-130">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="16bfe-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="16bfe-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="16bfe-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="16bfe-132">7 </span><span class="sxs-lookup"><span data-stu-id="16bfe-132">7</span></span>|<span data-ttu-id="16bfe-133">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="16bfe-133">At least alphanumeric with symbols password required.</span></span>|



