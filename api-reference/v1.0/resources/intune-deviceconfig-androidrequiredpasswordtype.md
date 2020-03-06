---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e1ac4e27243adc47b087aa6453ff316d9b2e2fa1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530963"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="9ff15-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9ff15-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="9ff15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ff15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ff15-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ff15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ff15-106">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="9ff15-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="9ff15-107">成员</span><span class="sxs-lookup"><span data-stu-id="9ff15-107">Members</span></span>
|<span data-ttu-id="9ff15-108">成员</span><span class="sxs-lookup"><span data-stu-id="9ff15-108">Member</span></span>|<span data-ttu-id="9ff15-109">值</span><span class="sxs-lookup"><span data-stu-id="9ff15-109">Value</span></span>|<span data-ttu-id="9ff15-110">说明</span><span class="sxs-lookup"><span data-stu-id="9ff15-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ff15-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9ff15-111">deviceDefault</span></span>|<span data-ttu-id="9ff15-112">0</span><span class="sxs-lookup"><span data-stu-id="9ff15-112">0</span></span>|<span data-ttu-id="9ff15-113">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="9ff15-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="9ff15-114">字母</span><span class="sxs-lookup"><span data-stu-id="9ff15-114">alphabetic</span></span>|<span data-ttu-id="9ff15-115">1 </span><span class="sxs-lookup"><span data-stu-id="9ff15-115">1</span></span>|<span data-ttu-id="9ff15-116">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="9ff15-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="9ff15-117">字母数字</span><span class="sxs-lookup"><span data-stu-id="9ff15-117">alphanumeric</span></span>|<span data-ttu-id="9ff15-118">2 </span><span class="sxs-lookup"><span data-stu-id="9ff15-118">2</span></span>|<span data-ttu-id="9ff15-119">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="9ff15-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="9ff15-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="9ff15-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="9ff15-121">3 </span><span class="sxs-lookup"><span data-stu-id="9ff15-121">3</span></span>|<span data-ttu-id="9ff15-122">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="9ff15-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="9ff15-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="9ff15-123">lowSecurityBiometric</span></span>|<span data-ttu-id="9ff15-124">4 </span><span class="sxs-lookup"><span data-stu-id="9ff15-124">4</span></span>|<span data-ttu-id="9ff15-125">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="9ff15-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="9ff15-126">位数</span><span class="sxs-lookup"><span data-stu-id="9ff15-126">numeric</span></span>|<span data-ttu-id="9ff15-127">5 </span><span class="sxs-lookup"><span data-stu-id="9ff15-127">5</span></span>|<span data-ttu-id="9ff15-128">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="9ff15-128">Numeric password required.</span></span>|
|<span data-ttu-id="9ff15-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="9ff15-129">numericComplex</span></span>|<span data-ttu-id="9ff15-130">6 </span><span class="sxs-lookup"><span data-stu-id="9ff15-130">6</span></span>|<span data-ttu-id="9ff15-131">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="9ff15-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="9ff15-132">任意</span><span class="sxs-lookup"><span data-stu-id="9ff15-132">any</span></span>|<span data-ttu-id="9ff15-133">7 </span><span class="sxs-lookup"><span data-stu-id="9ff15-133">7</span></span>|<span data-ttu-id="9ff15-134">需要密码或模式，可以接受。</span><span class="sxs-lookup"><span data-stu-id="9ff15-134">A password or pattern is required, and any is acceptable.</span></span>|




