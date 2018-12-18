---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
author: tfitzmac
ms.openlocfilehash: e9b757dc86bf71462f7f987cedfcd9e04497880e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349215"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="4a463-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4a463-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="4a463-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4a463-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a463-105">Android 所需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="4a463-105">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="4a463-106">成员</span><span class="sxs-lookup"><span data-stu-id="4a463-106">Members</span></span>
|<span data-ttu-id="4a463-107">成员</span><span class="sxs-lookup"><span data-stu-id="4a463-107">Member</span></span>|<span data-ttu-id="4a463-108">值</span><span class="sxs-lookup"><span data-stu-id="4a463-108">Value</span></span>|<span data-ttu-id="4a463-109">说明</span><span class="sxs-lookup"><span data-stu-id="4a463-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a463-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4a463-110">deviceDefault</span></span>|<span data-ttu-id="4a463-111">0</span><span class="sxs-lookup"><span data-stu-id="4a463-111">0</span></span>|<span data-ttu-id="4a463-112">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="4a463-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="4a463-113">字母</span><span class="sxs-lookup"><span data-stu-id="4a463-113">alphabetic</span></span>|<span data-ttu-id="4a463-114">1</span><span class="sxs-lookup"><span data-stu-id="4a463-114">1</span></span>|<span data-ttu-id="4a463-115">所需的密码字母。</span><span class="sxs-lookup"><span data-stu-id="4a463-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="4a463-116">字母数字</span><span class="sxs-lookup"><span data-stu-id="4a463-116">alphanumeric</span></span>|<span data-ttu-id="4a463-117">2</span><span class="sxs-lookup"><span data-stu-id="4a463-117">2</span></span>|<span data-ttu-id="4a463-118">所需的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="4a463-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="4a463-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="4a463-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="4a463-120">3</span><span class="sxs-lookup"><span data-stu-id="4a463-120">3</span></span>|<span data-ttu-id="4a463-121">所需的符号密码全角字母数字。</span><span class="sxs-lookup"><span data-stu-id="4a463-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="4a463-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="4a463-122">lowSecurityBiometric</span></span>|<span data-ttu-id="4a463-123">4</span><span class="sxs-lookup"><span data-stu-id="4a463-123">4</span></span>|<span data-ttu-id="4a463-124">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="4a463-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="4a463-125">数值</span><span class="sxs-lookup"><span data-stu-id="4a463-125">numeric</span></span>|<span data-ttu-id="4a463-126">5</span><span class="sxs-lookup"><span data-stu-id="4a463-126">5</span></span>|<span data-ttu-id="4a463-127">所需的数字密码。</span><span class="sxs-lookup"><span data-stu-id="4a463-127">Numeric password required.</span></span>|
|<span data-ttu-id="4a463-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="4a463-128">numericComplex</span></span>|<span data-ttu-id="4a463-129">6</span><span class="sxs-lookup"><span data-stu-id="4a463-129">6</span></span>|<span data-ttu-id="4a463-130">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="4a463-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="4a463-131">任意</span><span class="sxs-lookup"><span data-stu-id="4a463-131">any</span></span>|<span data-ttu-id="4a463-132">7</span><span class="sxs-lookup"><span data-stu-id="4a463-132">7</span></span>|<span data-ttu-id="4a463-133">Password 或模式是必需的且任何可接受。</span><span class="sxs-lookup"><span data-stu-id="4a463-133">A password or pattern is required, and any is acceptable.</span></span>|



