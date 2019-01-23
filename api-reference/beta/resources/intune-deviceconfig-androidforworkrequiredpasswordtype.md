---
title: androidForWorkRequiredPasswordType 枚举类型
description: Android 的工作被必需的密码类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3da48449de63fa134c68e3f27fd415c286666e4e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419602"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="c0ede-103">androidForWorkRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c0ede-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="c0ede-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c0ede-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0ede-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c0ede-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0ede-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0ede-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0ede-107">Android 的工作被必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c0ede-107">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="c0ede-108">成员</span><span class="sxs-lookup"><span data-stu-id="c0ede-108">Members</span></span>
|<span data-ttu-id="c0ede-109">成员</span><span class="sxs-lookup"><span data-stu-id="c0ede-109">Member</span></span>|<span data-ttu-id="c0ede-110">值</span><span class="sxs-lookup"><span data-stu-id="c0ede-110">Value</span></span>|<span data-ttu-id="c0ede-111">说明</span><span class="sxs-lookup"><span data-stu-id="c0ede-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0ede-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c0ede-112">deviceDefault</span></span>|<span data-ttu-id="c0ede-113">0</span><span class="sxs-lookup"><span data-stu-id="c0ede-113">0</span></span>|<span data-ttu-id="c0ede-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="c0ede-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="c0ede-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="c0ede-115">lowSecurityBiometric</span></span>|<span data-ttu-id="c0ede-116">1</span><span class="sxs-lookup"><span data-stu-id="c0ede-116">1</span></span>|<span data-ttu-id="c0ede-117">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="c0ede-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="c0ede-118">必需</span><span class="sxs-lookup"><span data-stu-id="c0ede-118">required</span></span>|<span data-ttu-id="c0ede-119">2</span><span class="sxs-lookup"><span data-stu-id="c0ede-119">2</span></span>|<span data-ttu-id="c0ede-120">必需项。</span><span class="sxs-lookup"><span data-stu-id="c0ede-120">Required.</span></span>|
|<span data-ttu-id="c0ede-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="c0ede-121">atLeastNumeric</span></span>|<span data-ttu-id="c0ede-122">3</span><span class="sxs-lookup"><span data-stu-id="c0ede-122">3</span></span>|<span data-ttu-id="c0ede-123">所需的密码至少数值。</span><span class="sxs-lookup"><span data-stu-id="c0ede-123">At least numeric password required.</span></span>|
|<span data-ttu-id="c0ede-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="c0ede-124">numericComplex</span></span>|<span data-ttu-id="c0ede-125">4</span><span class="sxs-lookup"><span data-stu-id="c0ede-125">4</span></span>|<span data-ttu-id="c0ede-126">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="c0ede-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="c0ede-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="c0ede-127">atLeastAlphabetic</span></span>|<span data-ttu-id="c0ede-128">5</span><span class="sxs-lookup"><span data-stu-id="c0ede-128">5</span></span>|<span data-ttu-id="c0ede-129">所需的密码至少字母。</span><span class="sxs-lookup"><span data-stu-id="c0ede-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="c0ede-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="c0ede-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="c0ede-131">6</span><span class="sxs-lookup"><span data-stu-id="c0ede-131">6</span></span>|<span data-ttu-id="c0ede-132">所需的至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="c0ede-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="c0ede-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="c0ede-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="c0ede-134">7</span><span class="sxs-lookup"><span data-stu-id="c0ede-134">7</span></span>|<span data-ttu-id="c0ede-135">使用所需的符号密码至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="c0ede-135">At least alphanumeric with symbols password required.</span></span>|




