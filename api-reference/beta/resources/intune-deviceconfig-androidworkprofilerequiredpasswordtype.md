---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 822c2021040b0dc4e6eb827e9fec54a40b5cad64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062083"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="637c3-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="637c3-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="637c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="637c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="637c3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="637c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="637c3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="637c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="637c3-107">Android 工作配置文件必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="637c3-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="637c3-108">成员</span><span class="sxs-lookup"><span data-stu-id="637c3-108">Members</span></span>
|<span data-ttu-id="637c3-109">成员</span><span class="sxs-lookup"><span data-stu-id="637c3-109">Member</span></span>|<span data-ttu-id="637c3-110">值</span><span class="sxs-lookup"><span data-stu-id="637c3-110">Value</span></span>|<span data-ttu-id="637c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="637c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="637c3-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="637c3-112">deviceDefault</span></span>|<span data-ttu-id="637c3-113">0</span><span class="sxs-lookup"><span data-stu-id="637c3-113">0</span></span>|<span data-ttu-id="637c3-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="637c3-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="637c3-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="637c3-115">lowSecurityBiometric</span></span>|<span data-ttu-id="637c3-116">1 </span><span class="sxs-lookup"><span data-stu-id="637c3-116">1</span></span>|<span data-ttu-id="637c3-117">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="637c3-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="637c3-118">必需</span><span class="sxs-lookup"><span data-stu-id="637c3-118">required</span></span>|<span data-ttu-id="637c3-119">2 </span><span class="sxs-lookup"><span data-stu-id="637c3-119">2</span></span>|<span data-ttu-id="637c3-120">必需。</span><span class="sxs-lookup"><span data-stu-id="637c3-120">Required.</span></span>|
|<span data-ttu-id="637c3-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="637c3-121">atLeastNumeric</span></span>|<span data-ttu-id="637c3-122">第三章</span><span class="sxs-lookup"><span data-stu-id="637c3-122">3</span></span>|<span data-ttu-id="637c3-123">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="637c3-123">At least numeric password required.</span></span>|
|<span data-ttu-id="637c3-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="637c3-124">numericComplex</span></span>|<span data-ttu-id="637c3-125">4 </span><span class="sxs-lookup"><span data-stu-id="637c3-125">4</span></span>|<span data-ttu-id="637c3-126">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="637c3-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="637c3-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="637c3-127">atLeastAlphabetic</span></span>|<span data-ttu-id="637c3-128">5 </span><span class="sxs-lookup"><span data-stu-id="637c3-128">5</span></span>|<span data-ttu-id="637c3-129">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="637c3-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="637c3-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="637c3-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="637c3-131">6 </span><span class="sxs-lookup"><span data-stu-id="637c3-131">6</span></span>|<span data-ttu-id="637c3-132">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="637c3-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="637c3-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="637c3-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="637c3-134">7 </span><span class="sxs-lookup"><span data-stu-id="637c3-134">7</span></span>|<span data-ttu-id="637c3-135">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="637c3-135">At least alphanumeric with symbols password required.</span></span>|






