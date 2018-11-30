---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
ms.openlocfilehash: 96873cdc228759ea1354c7f55d97ba1046ffb2e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043159"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="b24ce-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b24ce-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="b24ce-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b24ce-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b24ce-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b24ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b24ce-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b24ce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b24ce-107">Android 所需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="b24ce-107">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="b24ce-108">成员</span><span class="sxs-lookup"><span data-stu-id="b24ce-108">Members</span></span>
|<span data-ttu-id="b24ce-109">成员</span><span class="sxs-lookup"><span data-stu-id="b24ce-109">Member</span></span>|<span data-ttu-id="b24ce-110">值</span><span class="sxs-lookup"><span data-stu-id="b24ce-110">Value</span></span>|<span data-ttu-id="b24ce-111">说明</span><span class="sxs-lookup"><span data-stu-id="b24ce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b24ce-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b24ce-112">deviceDefault</span></span>|<span data-ttu-id="b24ce-113">0</span><span class="sxs-lookup"><span data-stu-id="b24ce-113">0</span></span>|<span data-ttu-id="b24ce-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="b24ce-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="b24ce-115">字母</span><span class="sxs-lookup"><span data-stu-id="b24ce-115">alphabetic</span></span>|<span data-ttu-id="b24ce-116">1</span><span class="sxs-lookup"><span data-stu-id="b24ce-116">1</span></span>|<span data-ttu-id="b24ce-117">所需的密码字母。</span><span class="sxs-lookup"><span data-stu-id="b24ce-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="b24ce-118">字母数字</span><span class="sxs-lookup"><span data-stu-id="b24ce-118">alphanumeric</span></span>|<span data-ttu-id="b24ce-119">2</span><span class="sxs-lookup"><span data-stu-id="b24ce-119">2</span></span>|<span data-ttu-id="b24ce-120">所需的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="b24ce-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="b24ce-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="b24ce-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="b24ce-122">3</span><span class="sxs-lookup"><span data-stu-id="b24ce-122">3</span></span>|<span data-ttu-id="b24ce-123">所需的符号密码全角字母数字。</span><span class="sxs-lookup"><span data-stu-id="b24ce-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="b24ce-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="b24ce-124">lowSecurityBiometric</span></span>|<span data-ttu-id="b24ce-125">4</span><span class="sxs-lookup"><span data-stu-id="b24ce-125">4</span></span>|<span data-ttu-id="b24ce-126">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="b24ce-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="b24ce-127">数值</span><span class="sxs-lookup"><span data-stu-id="b24ce-127">numeric</span></span>|<span data-ttu-id="b24ce-128">5</span><span class="sxs-lookup"><span data-stu-id="b24ce-128">5</span></span>|<span data-ttu-id="b24ce-129">所需的数字密码。</span><span class="sxs-lookup"><span data-stu-id="b24ce-129">Numeric password required.</span></span>|
|<span data-ttu-id="b24ce-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="b24ce-130">numericComplex</span></span>|<span data-ttu-id="b24ce-131">6</span><span class="sxs-lookup"><span data-stu-id="b24ce-131">6</span></span>|<span data-ttu-id="b24ce-132">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="b24ce-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="b24ce-133">任意</span><span class="sxs-lookup"><span data-stu-id="b24ce-133">any</span></span>|<span data-ttu-id="b24ce-134">7</span><span class="sxs-lookup"><span data-stu-id="b24ce-134">7</span></span>|<span data-ttu-id="b24ce-135">Password 或模式是必需的且任何可接受。</span><span class="sxs-lookup"><span data-stu-id="b24ce-135">A password or pattern is required, and any is acceptable.</span></span>|





