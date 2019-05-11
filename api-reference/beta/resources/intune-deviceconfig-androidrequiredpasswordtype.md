---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8bcdf143e880940bd407d3c1d550b51ee491346c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33948497"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="12544-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="12544-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="12544-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12544-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12544-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12544-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12544-106">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="12544-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="12544-107">成员</span><span class="sxs-lookup"><span data-stu-id="12544-107">Members</span></span>
|<span data-ttu-id="12544-108">成员</span><span class="sxs-lookup"><span data-stu-id="12544-108">Member</span></span>|<span data-ttu-id="12544-109">值</span><span class="sxs-lookup"><span data-stu-id="12544-109">Value</span></span>|<span data-ttu-id="12544-110">说明</span><span class="sxs-lookup"><span data-stu-id="12544-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12544-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="12544-111">deviceDefault</span></span>|<span data-ttu-id="12544-112">0</span><span class="sxs-lookup"><span data-stu-id="12544-112">0</span></span>|<span data-ttu-id="12544-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="12544-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="12544-114">字母</span><span class="sxs-lookup"><span data-stu-id="12544-114">alphabetic</span></span>|<span data-ttu-id="12544-115">1</span><span class="sxs-lookup"><span data-stu-id="12544-115">1</span></span>|<span data-ttu-id="12544-116">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="12544-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="12544-117">字母数字</span><span class="sxs-lookup"><span data-stu-id="12544-117">alphanumeric</span></span>|<span data-ttu-id="12544-118">双面</span><span class="sxs-lookup"><span data-stu-id="12544-118">2</span></span>|<span data-ttu-id="12544-119">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="12544-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="12544-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="12544-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="12544-121">第三章</span><span class="sxs-lookup"><span data-stu-id="12544-121">3</span></span>|<span data-ttu-id="12544-122">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="12544-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="12544-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="12544-123">lowSecurityBiometric</span></span>|<span data-ttu-id="12544-124">4</span><span class="sxs-lookup"><span data-stu-id="12544-124">4</span></span>|<span data-ttu-id="12544-125">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="12544-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="12544-126">位数</span><span class="sxs-lookup"><span data-stu-id="12544-126">numeric</span></span>|<span data-ttu-id="12544-127">5</span><span class="sxs-lookup"><span data-stu-id="12544-127">5</span></span>|<span data-ttu-id="12544-128">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="12544-128">Numeric password required.</span></span>|
|<span data-ttu-id="12544-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="12544-129">numericComplex</span></span>|<span data-ttu-id="12544-130">型</span><span class="sxs-lookup"><span data-stu-id="12544-130">6</span></span>|<span data-ttu-id="12544-131">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="12544-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="12544-132">任意</span><span class="sxs-lookup"><span data-stu-id="12544-132">any</span></span>|<span data-ttu-id="12544-133">步</span><span class="sxs-lookup"><span data-stu-id="12544-133">7</span></span>|<span data-ttu-id="12544-134">需要密码或模式, 可以接受。</span><span class="sxs-lookup"><span data-stu-id="12544-134">A password or pattern is required, and any is acceptable.</span></span>|




