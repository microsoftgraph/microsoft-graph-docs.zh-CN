---
title: androidForWorkRequiredPasswordType 枚举类型
description: Android 的工作被必需的密码类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b7d64ce762b3c07af74e02ed0aa37accf615ef7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850209"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="0bb61-103">androidForWorkRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0bb61-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="0bb61-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0bb61-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bb61-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0bb61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bb61-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0bb61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bb61-107">Android 的工作被必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="0bb61-107">Android For Work required password type.</span></span>
## <a name="members"></a><span data-ttu-id="0bb61-108">成员</span><span class="sxs-lookup"><span data-stu-id="0bb61-108">Members</span></span>
|<span data-ttu-id="0bb61-109">成员</span><span class="sxs-lookup"><span data-stu-id="0bb61-109">Member</span></span>|<span data-ttu-id="0bb61-110">值</span><span class="sxs-lookup"><span data-stu-id="0bb61-110">Value</span></span>|<span data-ttu-id="0bb61-111">Description</span><span class="sxs-lookup"><span data-stu-id="0bb61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bb61-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="0bb61-112">deviceDefault</span></span>|<span data-ttu-id="0bb61-113">0</span><span class="sxs-lookup"><span data-stu-id="0bb61-113">0</span></span>|<span data-ttu-id="0bb61-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="0bb61-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="0bb61-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="0bb61-115">lowSecurityBiometric</span></span>|<span data-ttu-id="0bb61-116">1</span><span class="sxs-lookup"><span data-stu-id="0bb61-116">1</span></span>|<span data-ttu-id="0bb61-117">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="0bb61-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="0bb61-118">必需</span><span class="sxs-lookup"><span data-stu-id="0bb61-118">required</span></span>|<span data-ttu-id="0bb61-119">2</span><span class="sxs-lookup"><span data-stu-id="0bb61-119">2</span></span>|<span data-ttu-id="0bb61-120">必填。</span><span class="sxs-lookup"><span data-stu-id="0bb61-120">Required.</span></span>|
|<span data-ttu-id="0bb61-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="0bb61-121">atLeastNumeric</span></span>|<span data-ttu-id="0bb61-122">3</span><span class="sxs-lookup"><span data-stu-id="0bb61-122">3</span></span>|<span data-ttu-id="0bb61-123">所需的密码至少数值。</span><span class="sxs-lookup"><span data-stu-id="0bb61-123">At least numeric password required.</span></span>|
|<span data-ttu-id="0bb61-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="0bb61-124">numericComplex</span></span>|<span data-ttu-id="0bb61-125">4</span><span class="sxs-lookup"><span data-stu-id="0bb61-125">4</span></span>|<span data-ttu-id="0bb61-126">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="0bb61-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="0bb61-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="0bb61-127">atLeastAlphabetic</span></span>|<span data-ttu-id="0bb61-128">5</span><span class="sxs-lookup"><span data-stu-id="0bb61-128">5</span></span>|<span data-ttu-id="0bb61-129">所需的密码至少字母。</span><span class="sxs-lookup"><span data-stu-id="0bb61-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="0bb61-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="0bb61-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="0bb61-131">6</span><span class="sxs-lookup"><span data-stu-id="0bb61-131">6</span></span>|<span data-ttu-id="0bb61-132">所需的至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="0bb61-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="0bb61-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="0bb61-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="0bb61-134">7</span><span class="sxs-lookup"><span data-stu-id="0bb61-134">7</span></span>|<span data-ttu-id="0bb61-135">使用所需的符号密码至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="0bb61-135">At least alphanumeric with symbols password required.</span></span>|





