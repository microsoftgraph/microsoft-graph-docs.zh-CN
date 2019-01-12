---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作模板所需密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbe1eb1482e979d236c1f8bf92f687077fb189f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986276"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="09ffa-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="09ffa-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="09ffa-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="09ffa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09ffa-105">Android 工作模板所需密码类型。</span><span class="sxs-lookup"><span data-stu-id="09ffa-105">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="09ffa-106">成员</span><span class="sxs-lookup"><span data-stu-id="09ffa-106">Members</span></span>
|<span data-ttu-id="09ffa-107">成员</span><span class="sxs-lookup"><span data-stu-id="09ffa-107">Member</span></span>|<span data-ttu-id="09ffa-108">值</span><span class="sxs-lookup"><span data-stu-id="09ffa-108">Value</span></span>|<span data-ttu-id="09ffa-109">Description</span><span class="sxs-lookup"><span data-stu-id="09ffa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09ffa-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="09ffa-110">deviceDefault</span></span>|<span data-ttu-id="09ffa-111">0</span><span class="sxs-lookup"><span data-stu-id="09ffa-111">0</span></span>|<span data-ttu-id="09ffa-112">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="09ffa-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="09ffa-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="09ffa-113">lowSecurityBiometric</span></span>|<span data-ttu-id="09ffa-114">1</span><span class="sxs-lookup"><span data-stu-id="09ffa-114">1</span></span>|<span data-ttu-id="09ffa-115">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="09ffa-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="09ffa-116">必需</span><span class="sxs-lookup"><span data-stu-id="09ffa-116">required</span></span>|<span data-ttu-id="09ffa-117">2</span><span class="sxs-lookup"><span data-stu-id="09ffa-117">2</span></span>|<span data-ttu-id="09ffa-118">必填。</span><span class="sxs-lookup"><span data-stu-id="09ffa-118">Required.</span></span>|
|<span data-ttu-id="09ffa-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="09ffa-119">atLeastNumeric</span></span>|<span data-ttu-id="09ffa-120">3</span><span class="sxs-lookup"><span data-stu-id="09ffa-120">3</span></span>|<span data-ttu-id="09ffa-121">所需的密码至少数值。</span><span class="sxs-lookup"><span data-stu-id="09ffa-121">At least numeric password required.</span></span>|
|<span data-ttu-id="09ffa-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="09ffa-122">numericComplex</span></span>|<span data-ttu-id="09ffa-123">4</span><span class="sxs-lookup"><span data-stu-id="09ffa-123">4</span></span>|<span data-ttu-id="09ffa-124">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="09ffa-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="09ffa-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="09ffa-125">atLeastAlphabetic</span></span>|<span data-ttu-id="09ffa-126">5</span><span class="sxs-lookup"><span data-stu-id="09ffa-126">5</span></span>|<span data-ttu-id="09ffa-127">所需的密码至少字母。</span><span class="sxs-lookup"><span data-stu-id="09ffa-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="09ffa-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="09ffa-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="09ffa-129">6</span><span class="sxs-lookup"><span data-stu-id="09ffa-129">6</span></span>|<span data-ttu-id="09ffa-130">所需的至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="09ffa-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="09ffa-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="09ffa-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="09ffa-132">7</span><span class="sxs-lookup"><span data-stu-id="09ffa-132">7</span></span>|<span data-ttu-id="09ffa-133">使用所需的符号密码至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="09ffa-133">At least alphanumeric with symbols password required.</span></span>|



