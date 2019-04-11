---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d70ac87a0e8e3e8d97705b46f5d6ec63d85fbcac
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782070"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="6b3f2-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6b3f2-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="6b3f2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b3f2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b3f2-106">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="6b3f2-107">成员</span><span class="sxs-lookup"><span data-stu-id="6b3f2-107">Members</span></span>
|<span data-ttu-id="6b3f2-108">成员</span><span class="sxs-lookup"><span data-stu-id="6b3f2-108">Member</span></span>|<span data-ttu-id="6b3f2-109">值</span><span class="sxs-lookup"><span data-stu-id="6b3f2-109">Value</span></span>|<span data-ttu-id="6b3f2-110">说明</span><span class="sxs-lookup"><span data-stu-id="6b3f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b3f2-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="6b3f2-111">deviceDefault</span></span>|<span data-ttu-id="6b3f2-112">0</span><span class="sxs-lookup"><span data-stu-id="6b3f2-112">0</span></span>|<span data-ttu-id="6b3f2-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="6b3f2-114">字母</span><span class="sxs-lookup"><span data-stu-id="6b3f2-114">alphabetic</span></span>|<span data-ttu-id="6b3f2-115">1</span><span class="sxs-lookup"><span data-stu-id="6b3f2-115">1</span></span>|<span data-ttu-id="6b3f2-116">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="6b3f2-117">字母数字</span><span class="sxs-lookup"><span data-stu-id="6b3f2-117">alphanumeric</span></span>|<span data-ttu-id="6b3f2-118">双面</span><span class="sxs-lookup"><span data-stu-id="6b3f2-118">2</span></span>|<span data-ttu-id="6b3f2-119">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="6b3f2-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="6b3f2-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="6b3f2-121">第三章</span><span class="sxs-lookup"><span data-stu-id="6b3f2-121">3</span></span>|<span data-ttu-id="6b3f2-122">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="6b3f2-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="6b3f2-123">lowSecurityBiometric</span></span>|<span data-ttu-id="6b3f2-124">4</span><span class="sxs-lookup"><span data-stu-id="6b3f2-124">4</span></span>|<span data-ttu-id="6b3f2-125">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="6b3f2-126">位数</span><span class="sxs-lookup"><span data-stu-id="6b3f2-126">numeric</span></span>|<span data-ttu-id="6b3f2-127">5</span><span class="sxs-lookup"><span data-stu-id="6b3f2-127">5</span></span>|<span data-ttu-id="6b3f2-128">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-128">Numeric password required.</span></span>|
|<span data-ttu-id="6b3f2-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="6b3f2-129">numericComplex</span></span>|<span data-ttu-id="6b3f2-130">型</span><span class="sxs-lookup"><span data-stu-id="6b3f2-130">6</span></span>|<span data-ttu-id="6b3f2-131">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="6b3f2-132">任意</span><span class="sxs-lookup"><span data-stu-id="6b3f2-132">any</span></span>|<span data-ttu-id="6b3f2-133">步</span><span class="sxs-lookup"><span data-stu-id="6b3f2-133">7</span></span>|<span data-ttu-id="6b3f2-134">需要密码或模式, 可以接受。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-134">A password or pattern is required, and any is acceptable.</span></span>|





