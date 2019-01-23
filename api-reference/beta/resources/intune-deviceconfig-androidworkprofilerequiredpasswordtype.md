---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作模板所需密码类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cdf8c03dab6642cf6859ca822001a71b041c0e54
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399897"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="329bc-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="329bc-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="329bc-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="329bc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="329bc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="329bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="329bc-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="329bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="329bc-107">Android 工作模板所需密码类型。</span><span class="sxs-lookup"><span data-stu-id="329bc-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="329bc-108">成员</span><span class="sxs-lookup"><span data-stu-id="329bc-108">Members</span></span>
|<span data-ttu-id="329bc-109">成员</span><span class="sxs-lookup"><span data-stu-id="329bc-109">Member</span></span>|<span data-ttu-id="329bc-110">值</span><span class="sxs-lookup"><span data-stu-id="329bc-110">Value</span></span>|<span data-ttu-id="329bc-111">说明</span><span class="sxs-lookup"><span data-stu-id="329bc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="329bc-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="329bc-112">deviceDefault</span></span>|<span data-ttu-id="329bc-113">0</span><span class="sxs-lookup"><span data-stu-id="329bc-113">0</span></span>|<span data-ttu-id="329bc-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="329bc-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="329bc-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="329bc-115">lowSecurityBiometric</span></span>|<span data-ttu-id="329bc-116">1</span><span class="sxs-lookup"><span data-stu-id="329bc-116">1</span></span>|<span data-ttu-id="329bc-117">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="329bc-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="329bc-118">必需</span><span class="sxs-lookup"><span data-stu-id="329bc-118">required</span></span>|<span data-ttu-id="329bc-119">2</span><span class="sxs-lookup"><span data-stu-id="329bc-119">2</span></span>|<span data-ttu-id="329bc-120">必需项。</span><span class="sxs-lookup"><span data-stu-id="329bc-120">Required.</span></span>|
|<span data-ttu-id="329bc-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="329bc-121">atLeastNumeric</span></span>|<span data-ttu-id="329bc-122">3</span><span class="sxs-lookup"><span data-stu-id="329bc-122">3</span></span>|<span data-ttu-id="329bc-123">所需的密码至少数值。</span><span class="sxs-lookup"><span data-stu-id="329bc-123">At least numeric password required.</span></span>|
|<span data-ttu-id="329bc-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="329bc-124">numericComplex</span></span>|<span data-ttu-id="329bc-125">4</span><span class="sxs-lookup"><span data-stu-id="329bc-125">4</span></span>|<span data-ttu-id="329bc-126">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="329bc-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="329bc-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="329bc-127">atLeastAlphabetic</span></span>|<span data-ttu-id="329bc-128">5</span><span class="sxs-lookup"><span data-stu-id="329bc-128">5</span></span>|<span data-ttu-id="329bc-129">所需的密码至少字母。</span><span class="sxs-lookup"><span data-stu-id="329bc-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="329bc-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="329bc-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="329bc-131">6</span><span class="sxs-lookup"><span data-stu-id="329bc-131">6</span></span>|<span data-ttu-id="329bc-132">所需的至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="329bc-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="329bc-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="329bc-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="329bc-134">7</span><span class="sxs-lookup"><span data-stu-id="329bc-134">7</span></span>|<span data-ttu-id="329bc-135">使用所需的符号密码至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="329bc-135">At least alphanumeric with symbols password required.</span></span>|




