---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4c87a56e6b53654597a41742d835d7de5eaddcc2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051163"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="32b35-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="32b35-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="32b35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32b35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32b35-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32b35-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32b35-106">Android 工作配置文件必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="32b35-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="32b35-107">成员</span><span class="sxs-lookup"><span data-stu-id="32b35-107">Members</span></span>
|<span data-ttu-id="32b35-108">成员</span><span class="sxs-lookup"><span data-stu-id="32b35-108">Member</span></span>|<span data-ttu-id="32b35-109">值</span><span class="sxs-lookup"><span data-stu-id="32b35-109">Value</span></span>|<span data-ttu-id="32b35-110">说明</span><span class="sxs-lookup"><span data-stu-id="32b35-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32b35-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="32b35-111">deviceDefault</span></span>|<span data-ttu-id="32b35-112">0</span><span class="sxs-lookup"><span data-stu-id="32b35-112">0</span></span>|<span data-ttu-id="32b35-113">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="32b35-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="32b35-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="32b35-114">lowSecurityBiometric</span></span>|<span data-ttu-id="32b35-115">1 </span><span class="sxs-lookup"><span data-stu-id="32b35-115">1</span></span>|<span data-ttu-id="32b35-116">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="32b35-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="32b35-117">必需</span><span class="sxs-lookup"><span data-stu-id="32b35-117">required</span></span>|<span data-ttu-id="32b35-118">2 </span><span class="sxs-lookup"><span data-stu-id="32b35-118">2</span></span>|<span data-ttu-id="32b35-119">必需。</span><span class="sxs-lookup"><span data-stu-id="32b35-119">Required.</span></span>|
|<span data-ttu-id="32b35-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="32b35-120">atLeastNumeric</span></span>|<span data-ttu-id="32b35-121">第三章</span><span class="sxs-lookup"><span data-stu-id="32b35-121">3</span></span>|<span data-ttu-id="32b35-122">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="32b35-122">At least numeric password required.</span></span>|
|<span data-ttu-id="32b35-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="32b35-123">numericComplex</span></span>|<span data-ttu-id="32b35-124">4 </span><span class="sxs-lookup"><span data-stu-id="32b35-124">4</span></span>|<span data-ttu-id="32b35-125">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="32b35-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="32b35-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="32b35-126">atLeastAlphabetic</span></span>|<span data-ttu-id="32b35-127">5 </span><span class="sxs-lookup"><span data-stu-id="32b35-127">5</span></span>|<span data-ttu-id="32b35-128">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="32b35-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="32b35-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="32b35-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="32b35-130">6 </span><span class="sxs-lookup"><span data-stu-id="32b35-130">6</span></span>|<span data-ttu-id="32b35-131">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="32b35-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="32b35-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="32b35-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="32b35-133">7 </span><span class="sxs-lookup"><span data-stu-id="32b35-133">7</span></span>|<span data-ttu-id="32b35-134">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="32b35-134">At least alphanumeric with symbols password required.</span></span>|









