---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作模板所需密码类型。
author: tfitzmac
ms.openlocfilehash: 64b5dfcd5b919a428ef6823856dbf67102a316c2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331659"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="a71d8-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a71d8-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="a71d8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a71d8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a71d8-105">Android 工作模板所需密码类型。</span><span class="sxs-lookup"><span data-stu-id="a71d8-105">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="a71d8-106">成员</span><span class="sxs-lookup"><span data-stu-id="a71d8-106">Members</span></span>
|<span data-ttu-id="a71d8-107">成员</span><span class="sxs-lookup"><span data-stu-id="a71d8-107">Member</span></span>|<span data-ttu-id="a71d8-108">值</span><span class="sxs-lookup"><span data-stu-id="a71d8-108">Value</span></span>|<span data-ttu-id="a71d8-109">说明</span><span class="sxs-lookup"><span data-stu-id="a71d8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a71d8-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a71d8-110">deviceDefault</span></span>|<span data-ttu-id="a71d8-111">0</span><span class="sxs-lookup"><span data-stu-id="a71d8-111">0</span></span>|<span data-ttu-id="a71d8-112">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="a71d8-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="a71d8-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="a71d8-113">lowSecurityBiometric</span></span>|<span data-ttu-id="a71d8-114">1</span><span class="sxs-lookup"><span data-stu-id="a71d8-114">1</span></span>|<span data-ttu-id="a71d8-115">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="a71d8-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="a71d8-116">必需</span><span class="sxs-lookup"><span data-stu-id="a71d8-116">required</span></span>|<span data-ttu-id="a71d8-117">2</span><span class="sxs-lookup"><span data-stu-id="a71d8-117">2</span></span>|<span data-ttu-id="a71d8-118">必需。</span><span class="sxs-lookup"><span data-stu-id="a71d8-118">Required.</span></span>|
|<span data-ttu-id="a71d8-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="a71d8-119">atLeastNumeric</span></span>|<span data-ttu-id="a71d8-120">3</span><span class="sxs-lookup"><span data-stu-id="a71d8-120">3</span></span>|<span data-ttu-id="a71d8-121">所需的密码至少数值。</span><span class="sxs-lookup"><span data-stu-id="a71d8-121">At least numeric password required.</span></span>|
|<span data-ttu-id="a71d8-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="a71d8-122">numericComplex</span></span>|<span data-ttu-id="a71d8-123">4</span><span class="sxs-lookup"><span data-stu-id="a71d8-123">4</span></span>|<span data-ttu-id="a71d8-124">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="a71d8-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="a71d8-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="a71d8-125">atLeastAlphabetic</span></span>|<span data-ttu-id="a71d8-126">5</span><span class="sxs-lookup"><span data-stu-id="a71d8-126">5</span></span>|<span data-ttu-id="a71d8-127">所需的密码至少字母。</span><span class="sxs-lookup"><span data-stu-id="a71d8-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="a71d8-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="a71d8-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="a71d8-129">6</span><span class="sxs-lookup"><span data-stu-id="a71d8-129">6</span></span>|<span data-ttu-id="a71d8-130">所需的至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="a71d8-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="a71d8-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="a71d8-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="a71d8-132">7</span><span class="sxs-lookup"><span data-stu-id="a71d8-132">7</span></span>|<span data-ttu-id="a71d8-133">使用所需的符号密码至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="a71d8-133">At least alphanumeric with symbols password required.</span></span>|



