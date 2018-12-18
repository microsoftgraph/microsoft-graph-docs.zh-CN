---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作模板所需密码类型。
author: tfitzmac
ms.openlocfilehash: 8d41b4c516ee4aa393ea3a26034e5f575b58fa02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330231"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="469e4-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="469e4-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="469e4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="469e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="469e4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="469e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="469e4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="469e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="469e4-107">Android 工作模板所需密码类型。</span><span class="sxs-lookup"><span data-stu-id="469e4-107">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="469e4-108">成员</span><span class="sxs-lookup"><span data-stu-id="469e4-108">Members</span></span>
|<span data-ttu-id="469e4-109">成员</span><span class="sxs-lookup"><span data-stu-id="469e4-109">Member</span></span>|<span data-ttu-id="469e4-110">值</span><span class="sxs-lookup"><span data-stu-id="469e4-110">Value</span></span>|<span data-ttu-id="469e4-111">说明</span><span class="sxs-lookup"><span data-stu-id="469e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="469e4-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="469e4-112">deviceDefault</span></span>|<span data-ttu-id="469e4-113">0</span><span class="sxs-lookup"><span data-stu-id="469e4-113">0</span></span>|<span data-ttu-id="469e4-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="469e4-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="469e4-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="469e4-115">lowSecurityBiometric</span></span>|<span data-ttu-id="469e4-116">1</span><span class="sxs-lookup"><span data-stu-id="469e4-116">1</span></span>|<span data-ttu-id="469e4-117">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="469e4-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="469e4-118">必需</span><span class="sxs-lookup"><span data-stu-id="469e4-118">required</span></span>|<span data-ttu-id="469e4-119">2</span><span class="sxs-lookup"><span data-stu-id="469e4-119">2</span></span>|<span data-ttu-id="469e4-120">必需。</span><span class="sxs-lookup"><span data-stu-id="469e4-120">Required.</span></span>|
|<span data-ttu-id="469e4-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="469e4-121">atLeastNumeric</span></span>|<span data-ttu-id="469e4-122">3</span><span class="sxs-lookup"><span data-stu-id="469e4-122">3</span></span>|<span data-ttu-id="469e4-123">所需的密码至少数值。</span><span class="sxs-lookup"><span data-stu-id="469e4-123">At least numeric password required.</span></span>|
|<span data-ttu-id="469e4-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="469e4-124">numericComplex</span></span>|<span data-ttu-id="469e4-125">4</span><span class="sxs-lookup"><span data-stu-id="469e4-125">4</span></span>|<span data-ttu-id="469e4-126">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="469e4-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="469e4-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="469e4-127">atLeastAlphabetic</span></span>|<span data-ttu-id="469e4-128">5</span><span class="sxs-lookup"><span data-stu-id="469e4-128">5</span></span>|<span data-ttu-id="469e4-129">所需的密码至少字母。</span><span class="sxs-lookup"><span data-stu-id="469e4-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="469e4-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="469e4-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="469e4-131">6</span><span class="sxs-lookup"><span data-stu-id="469e4-131">6</span></span>|<span data-ttu-id="469e4-132">所需的至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="469e4-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="469e4-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="469e4-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="469e4-134">7</span><span class="sxs-lookup"><span data-stu-id="469e4-134">7</span></span>|<span data-ttu-id="469e4-135">使用所需的符号密码至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="469e4-135">At least alphanumeric with symbols password required.</span></span>|





