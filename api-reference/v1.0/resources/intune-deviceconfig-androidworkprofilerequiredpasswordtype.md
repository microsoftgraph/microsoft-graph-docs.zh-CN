---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作模板所需密码类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c77b9b3265a5c3f64da93df58d5a605923dff69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809930"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="c9f00-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c9f00-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="c9f00-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c9f00-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9f00-105">Android 工作模板所需密码类型。</span><span class="sxs-lookup"><span data-stu-id="c9f00-105">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="c9f00-106">成员</span><span class="sxs-lookup"><span data-stu-id="c9f00-106">Members</span></span>
|<span data-ttu-id="c9f00-107">成员</span><span class="sxs-lookup"><span data-stu-id="c9f00-107">Member</span></span>|<span data-ttu-id="c9f00-108">值</span><span class="sxs-lookup"><span data-stu-id="c9f00-108">Value</span></span>|<span data-ttu-id="c9f00-109">Description</span><span class="sxs-lookup"><span data-stu-id="c9f00-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9f00-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c9f00-110">deviceDefault</span></span>|<span data-ttu-id="c9f00-111">0</span><span class="sxs-lookup"><span data-stu-id="c9f00-111">0</span></span>|<span data-ttu-id="c9f00-112">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="c9f00-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="c9f00-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="c9f00-113">lowSecurityBiometric</span></span>|<span data-ttu-id="c9f00-114">1</span><span class="sxs-lookup"><span data-stu-id="c9f00-114">1</span></span>|<span data-ttu-id="c9f00-115">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="c9f00-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="c9f00-116">必需</span><span class="sxs-lookup"><span data-stu-id="c9f00-116">required</span></span>|<span data-ttu-id="c9f00-117">2</span><span class="sxs-lookup"><span data-stu-id="c9f00-117">2</span></span>|<span data-ttu-id="c9f00-118">必填。</span><span class="sxs-lookup"><span data-stu-id="c9f00-118">Required.</span></span>|
|<span data-ttu-id="c9f00-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="c9f00-119">atLeastNumeric</span></span>|<span data-ttu-id="c9f00-120">3</span><span class="sxs-lookup"><span data-stu-id="c9f00-120">3</span></span>|<span data-ttu-id="c9f00-121">所需的密码至少数值。</span><span class="sxs-lookup"><span data-stu-id="c9f00-121">At least numeric password required.</span></span>|
|<span data-ttu-id="c9f00-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="c9f00-122">numericComplex</span></span>|<span data-ttu-id="c9f00-123">4</span><span class="sxs-lookup"><span data-stu-id="c9f00-123">4</span></span>|<span data-ttu-id="c9f00-124">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="c9f00-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="c9f00-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="c9f00-125">atLeastAlphabetic</span></span>|<span data-ttu-id="c9f00-126">5</span><span class="sxs-lookup"><span data-stu-id="c9f00-126">5</span></span>|<span data-ttu-id="c9f00-127">所需的密码至少字母。</span><span class="sxs-lookup"><span data-stu-id="c9f00-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="c9f00-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="c9f00-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="c9f00-129">6</span><span class="sxs-lookup"><span data-stu-id="c9f00-129">6</span></span>|<span data-ttu-id="c9f00-130">所需的至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="c9f00-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="c9f00-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="c9f00-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="c9f00-132">7</span><span class="sxs-lookup"><span data-stu-id="c9f00-132">7</span></span>|<span data-ttu-id="c9f00-133">使用所需的符号密码至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="c9f00-133">At least alphanumeric with symbols password required.</span></span>|



