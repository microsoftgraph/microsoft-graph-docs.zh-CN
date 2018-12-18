---
title: androidForWorkRequiredPasswordType 枚举类型
description: Android 的工作被必需的密码类型。
author: tfitzmac
ms.openlocfilehash: cefb41dea7a92f1b1a640d8c9bf701a321ad9ead
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357279"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="406d9-103">androidForWorkRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="406d9-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="406d9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="406d9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="406d9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="406d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="406d9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="406d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="406d9-107">Android 的工作被必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="406d9-107">Android For Work required password type.</span></span>
## <a name="members"></a><span data-ttu-id="406d9-108">成员</span><span class="sxs-lookup"><span data-stu-id="406d9-108">Members</span></span>
|<span data-ttu-id="406d9-109">成员</span><span class="sxs-lookup"><span data-stu-id="406d9-109">Member</span></span>|<span data-ttu-id="406d9-110">值</span><span class="sxs-lookup"><span data-stu-id="406d9-110">Value</span></span>|<span data-ttu-id="406d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="406d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="406d9-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="406d9-112">deviceDefault</span></span>|<span data-ttu-id="406d9-113">0</span><span class="sxs-lookup"><span data-stu-id="406d9-113">0</span></span>|<span data-ttu-id="406d9-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="406d9-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="406d9-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="406d9-115">lowSecurityBiometric</span></span>|<span data-ttu-id="406d9-116">1</span><span class="sxs-lookup"><span data-stu-id="406d9-116">1</span></span>|<span data-ttu-id="406d9-117">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="406d9-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="406d9-118">必需</span><span class="sxs-lookup"><span data-stu-id="406d9-118">required</span></span>|<span data-ttu-id="406d9-119">2</span><span class="sxs-lookup"><span data-stu-id="406d9-119">2</span></span>|<span data-ttu-id="406d9-120">必需。</span><span class="sxs-lookup"><span data-stu-id="406d9-120">Required.</span></span>|
|<span data-ttu-id="406d9-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="406d9-121">atLeastNumeric</span></span>|<span data-ttu-id="406d9-122">3</span><span class="sxs-lookup"><span data-stu-id="406d9-122">3</span></span>|<span data-ttu-id="406d9-123">所需的密码至少数值。</span><span class="sxs-lookup"><span data-stu-id="406d9-123">At least numeric password required.</span></span>|
|<span data-ttu-id="406d9-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="406d9-124">numericComplex</span></span>|<span data-ttu-id="406d9-125">4</span><span class="sxs-lookup"><span data-stu-id="406d9-125">4</span></span>|<span data-ttu-id="406d9-126">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="406d9-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="406d9-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="406d9-127">atLeastAlphabetic</span></span>|<span data-ttu-id="406d9-128">5</span><span class="sxs-lookup"><span data-stu-id="406d9-128">5</span></span>|<span data-ttu-id="406d9-129">所需的密码至少字母。</span><span class="sxs-lookup"><span data-stu-id="406d9-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="406d9-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="406d9-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="406d9-131">6</span><span class="sxs-lookup"><span data-stu-id="406d9-131">6</span></span>|<span data-ttu-id="406d9-132">所需的至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="406d9-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="406d9-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="406d9-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="406d9-134">7</span><span class="sxs-lookup"><span data-stu-id="406d9-134">7</span></span>|<span data-ttu-id="406d9-135">使用所需的符号密码至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="406d9-135">At least alphanumeric with symbols password required.</span></span>|





