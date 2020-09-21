---
title: androidForWorkRequiredPasswordType 枚举类型
description: 适用于工作所需密码类型的 Android。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 20c7e330d060346557717e9eea0924b275c60d04
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968491"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="4b7a2-103">androidForWorkRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4b7a2-103">androidForWorkRequiredPasswordType enum type</span></span>

<span data-ttu-id="4b7a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b7a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b7a2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4b7a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b7a2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b7a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b7a2-107">适用于工作所需密码类型的 Android。</span><span class="sxs-lookup"><span data-stu-id="4b7a2-107">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="4b7a2-108">成员</span><span class="sxs-lookup"><span data-stu-id="4b7a2-108">Members</span></span>
|<span data-ttu-id="4b7a2-109">成员</span><span class="sxs-lookup"><span data-stu-id="4b7a2-109">Member</span></span>|<span data-ttu-id="4b7a2-110">值</span><span class="sxs-lookup"><span data-stu-id="4b7a2-110">Value</span></span>|<span data-ttu-id="4b7a2-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b7a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b7a2-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4b7a2-112">deviceDefault</span></span>|<span data-ttu-id="4b7a2-113">0</span><span class="sxs-lookup"><span data-stu-id="4b7a2-113">0</span></span>|<span data-ttu-id="4b7a2-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="4b7a2-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="4b7a2-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="4b7a2-115">lowSecurityBiometric</span></span>|<span data-ttu-id="4b7a2-116">1 </span><span class="sxs-lookup"><span data-stu-id="4b7a2-116">1</span></span>|<span data-ttu-id="4b7a2-117">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="4b7a2-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="4b7a2-118">必需</span><span class="sxs-lookup"><span data-stu-id="4b7a2-118">required</span></span>|<span data-ttu-id="4b7a2-119">2 </span><span class="sxs-lookup"><span data-stu-id="4b7a2-119">2</span></span>|<span data-ttu-id="4b7a2-120">必需。</span><span class="sxs-lookup"><span data-stu-id="4b7a2-120">Required.</span></span>|
|<span data-ttu-id="4b7a2-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="4b7a2-121">atLeastNumeric</span></span>|<span data-ttu-id="4b7a2-122">第三章</span><span class="sxs-lookup"><span data-stu-id="4b7a2-122">3</span></span>|<span data-ttu-id="4b7a2-123">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="4b7a2-123">At least numeric password required.</span></span>|
|<span data-ttu-id="4b7a2-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="4b7a2-124">numericComplex</span></span>|<span data-ttu-id="4b7a2-125">4 </span><span class="sxs-lookup"><span data-stu-id="4b7a2-125">4</span></span>|<span data-ttu-id="4b7a2-126">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="4b7a2-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="4b7a2-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="4b7a2-127">atLeastAlphabetic</span></span>|<span data-ttu-id="4b7a2-128">5 </span><span class="sxs-lookup"><span data-stu-id="4b7a2-128">5</span></span>|<span data-ttu-id="4b7a2-129">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="4b7a2-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="4b7a2-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="4b7a2-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="4b7a2-131">6 </span><span class="sxs-lookup"><span data-stu-id="4b7a2-131">6</span></span>|<span data-ttu-id="4b7a2-132">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="4b7a2-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="4b7a2-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="4b7a2-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="4b7a2-134">7 </span><span class="sxs-lookup"><span data-stu-id="4b7a2-134">7</span></span>|<span data-ttu-id="4b7a2-135">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="4b7a2-135">At least alphanumeric with symbols password required.</span></span>|






