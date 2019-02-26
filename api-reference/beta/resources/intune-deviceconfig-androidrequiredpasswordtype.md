---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1845656d43ec2a8f567506ed61b5ee3bc6d8a9ad
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151518"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="49375-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="49375-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="49375-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="49375-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49375-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49375-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49375-106">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="49375-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="49375-107">成员</span><span class="sxs-lookup"><span data-stu-id="49375-107">Members</span></span>
|<span data-ttu-id="49375-108">成员</span><span class="sxs-lookup"><span data-stu-id="49375-108">Member</span></span>|<span data-ttu-id="49375-109">值</span><span class="sxs-lookup"><span data-stu-id="49375-109">Value</span></span>|<span data-ttu-id="49375-110">说明</span><span class="sxs-lookup"><span data-stu-id="49375-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49375-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="49375-111">deviceDefault</span></span>|<span data-ttu-id="49375-112">0</span><span class="sxs-lookup"><span data-stu-id="49375-112">0</span></span>|<span data-ttu-id="49375-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="49375-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="49375-114">字母</span><span class="sxs-lookup"><span data-stu-id="49375-114">alphabetic</span></span>|<span data-ttu-id="49375-115">1</span><span class="sxs-lookup"><span data-stu-id="49375-115">1</span></span>|<span data-ttu-id="49375-116">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="49375-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="49375-117">字母数字</span><span class="sxs-lookup"><span data-stu-id="49375-117">alphanumeric</span></span>|<span data-ttu-id="49375-118">双面</span><span class="sxs-lookup"><span data-stu-id="49375-118">2</span></span>|<span data-ttu-id="49375-119">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="49375-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="49375-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="49375-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="49375-121">第三章</span><span class="sxs-lookup"><span data-stu-id="49375-121">3</span></span>|<span data-ttu-id="49375-122">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="49375-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="49375-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="49375-123">lowSecurityBiometric</span></span>|<span data-ttu-id="49375-124">4</span><span class="sxs-lookup"><span data-stu-id="49375-124">4</span></span>|<span data-ttu-id="49375-125">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="49375-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="49375-126">位数</span><span class="sxs-lookup"><span data-stu-id="49375-126">numeric</span></span>|<span data-ttu-id="49375-127">5</span><span class="sxs-lookup"><span data-stu-id="49375-127">5</span></span>|<span data-ttu-id="49375-128">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="49375-128">Numeric password required.</span></span>|
|<span data-ttu-id="49375-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="49375-129">numericComplex</span></span>|<span data-ttu-id="49375-130">型</span><span class="sxs-lookup"><span data-stu-id="49375-130">6</span></span>|<span data-ttu-id="49375-131">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="49375-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="49375-132">任意</span><span class="sxs-lookup"><span data-stu-id="49375-132">any</span></span>|<span data-ttu-id="49375-133">步</span><span class="sxs-lookup"><span data-stu-id="49375-133">7</span></span>|<span data-ttu-id="49375-134">需要密码或模式, 可以接受。</span><span class="sxs-lookup"><span data-stu-id="49375-134">A password or pattern is required, and any is acceptable.</span></span>|




