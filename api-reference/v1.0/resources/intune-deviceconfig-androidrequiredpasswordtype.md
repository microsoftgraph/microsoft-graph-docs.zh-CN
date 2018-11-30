---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
ms.openlocfilehash: f4f95308791aa443b6eb4b4fd38c70fe2d47b4b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010724"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="b3084-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b3084-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="b3084-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b3084-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3084-105">Android 所需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="b3084-105">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="b3084-106">成员</span><span class="sxs-lookup"><span data-stu-id="b3084-106">Members</span></span>
|<span data-ttu-id="b3084-107">成员</span><span class="sxs-lookup"><span data-stu-id="b3084-107">Member</span></span>|<span data-ttu-id="b3084-108">值</span><span class="sxs-lookup"><span data-stu-id="b3084-108">Value</span></span>|<span data-ttu-id="b3084-109">说明</span><span class="sxs-lookup"><span data-stu-id="b3084-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3084-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b3084-110">deviceDefault</span></span>|<span data-ttu-id="b3084-111">0</span><span class="sxs-lookup"><span data-stu-id="b3084-111">0</span></span>|<span data-ttu-id="b3084-112">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="b3084-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="b3084-113">字母</span><span class="sxs-lookup"><span data-stu-id="b3084-113">alphabetic</span></span>|<span data-ttu-id="b3084-114">1</span><span class="sxs-lookup"><span data-stu-id="b3084-114">1</span></span>|<span data-ttu-id="b3084-115">所需的密码字母。</span><span class="sxs-lookup"><span data-stu-id="b3084-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="b3084-116">字母数字</span><span class="sxs-lookup"><span data-stu-id="b3084-116">alphanumeric</span></span>|<span data-ttu-id="b3084-117">2</span><span class="sxs-lookup"><span data-stu-id="b3084-117">2</span></span>|<span data-ttu-id="b3084-118">所需的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="b3084-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="b3084-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="b3084-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="b3084-120">3</span><span class="sxs-lookup"><span data-stu-id="b3084-120">3</span></span>|<span data-ttu-id="b3084-121">所需的符号密码全角字母数字。</span><span class="sxs-lookup"><span data-stu-id="b3084-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="b3084-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="b3084-122">lowSecurityBiometric</span></span>|<span data-ttu-id="b3084-123">4</span><span class="sxs-lookup"><span data-stu-id="b3084-123">4</span></span>|<span data-ttu-id="b3084-124">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="b3084-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="b3084-125">数值</span><span class="sxs-lookup"><span data-stu-id="b3084-125">numeric</span></span>|<span data-ttu-id="b3084-126">5</span><span class="sxs-lookup"><span data-stu-id="b3084-126">5</span></span>|<span data-ttu-id="b3084-127">所需的数字密码。</span><span class="sxs-lookup"><span data-stu-id="b3084-127">Numeric password required.</span></span>|
|<span data-ttu-id="b3084-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="b3084-128">numericComplex</span></span>|<span data-ttu-id="b3084-129">6</span><span class="sxs-lookup"><span data-stu-id="b3084-129">6</span></span>|<span data-ttu-id="b3084-130">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="b3084-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="b3084-131">任意</span><span class="sxs-lookup"><span data-stu-id="b3084-131">any</span></span>|<span data-ttu-id="b3084-132">7</span><span class="sxs-lookup"><span data-stu-id="b3084-132">7</span></span>|<span data-ttu-id="b3084-133">Password 或模式是必需的且任何可接受。</span><span class="sxs-lookup"><span data-stu-id="b3084-133">A password or pattern is required, and any is acceptable.</span></span>|



