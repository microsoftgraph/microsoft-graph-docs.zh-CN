---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作模板所需密码类型。
ms.openlocfilehash: f9cdf225f9fe7dfc42fb728bad615a7abde11bef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008075"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="864f5-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="864f5-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="864f5-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="864f5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="864f5-105">Android 工作模板所需密码类型。</span><span class="sxs-lookup"><span data-stu-id="864f5-105">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="864f5-106">成员</span><span class="sxs-lookup"><span data-stu-id="864f5-106">Members</span></span>
|<span data-ttu-id="864f5-107">成员</span><span class="sxs-lookup"><span data-stu-id="864f5-107">Member</span></span>|<span data-ttu-id="864f5-108">值</span><span class="sxs-lookup"><span data-stu-id="864f5-108">Value</span></span>|<span data-ttu-id="864f5-109">说明</span><span class="sxs-lookup"><span data-stu-id="864f5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="864f5-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="864f5-110">deviceDefault</span></span>|<span data-ttu-id="864f5-111">0</span><span class="sxs-lookup"><span data-stu-id="864f5-111">0</span></span>|<span data-ttu-id="864f5-112">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="864f5-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="864f5-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="864f5-113">lowSecurityBiometric</span></span>|<span data-ttu-id="864f5-114">1</span><span class="sxs-lookup"><span data-stu-id="864f5-114">1</span></span>|<span data-ttu-id="864f5-115">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="864f5-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="864f5-116">必需</span><span class="sxs-lookup"><span data-stu-id="864f5-116">required</span></span>|<span data-ttu-id="864f5-117">2</span><span class="sxs-lookup"><span data-stu-id="864f5-117">2</span></span>|<span data-ttu-id="864f5-118">必需。</span><span class="sxs-lookup"><span data-stu-id="864f5-118">Required.</span></span>|
|<span data-ttu-id="864f5-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="864f5-119">atLeastNumeric</span></span>|<span data-ttu-id="864f5-120">3</span><span class="sxs-lookup"><span data-stu-id="864f5-120">3</span></span>|<span data-ttu-id="864f5-121">所需的密码至少数值。</span><span class="sxs-lookup"><span data-stu-id="864f5-121">At least numeric password required.</span></span>|
|<span data-ttu-id="864f5-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="864f5-122">numericComplex</span></span>|<span data-ttu-id="864f5-123">4</span><span class="sxs-lookup"><span data-stu-id="864f5-123">4</span></span>|<span data-ttu-id="864f5-124">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="864f5-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="864f5-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="864f5-125">atLeastAlphabetic</span></span>|<span data-ttu-id="864f5-126">5</span><span class="sxs-lookup"><span data-stu-id="864f5-126">5</span></span>|<span data-ttu-id="864f5-127">所需的密码至少字母。</span><span class="sxs-lookup"><span data-stu-id="864f5-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="864f5-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="864f5-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="864f5-129">6</span><span class="sxs-lookup"><span data-stu-id="864f5-129">6</span></span>|<span data-ttu-id="864f5-130">所需的至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="864f5-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="864f5-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="864f5-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="864f5-132">7</span><span class="sxs-lookup"><span data-stu-id="864f5-132">7</span></span>|<span data-ttu-id="864f5-133">使用所需的符号密码至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="864f5-133">At least alphanumeric with symbols password required.</span></span>|



