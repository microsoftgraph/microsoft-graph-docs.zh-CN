---
title: androidForWorkRequiredPasswordType 枚举类型
description: 适用于工作所需密码类型的 Android。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab11ed4951fb61e96afc55381986e83fad7ce440
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991056"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="5ec65-103">androidForWorkRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5ec65-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="5ec65-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ec65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ec65-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ec65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ec65-106">适用于工作所需密码类型的 Android。</span><span class="sxs-lookup"><span data-stu-id="5ec65-106">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="5ec65-107">成员</span><span class="sxs-lookup"><span data-stu-id="5ec65-107">Members</span></span>
|<span data-ttu-id="5ec65-108">成员</span><span class="sxs-lookup"><span data-stu-id="5ec65-108">Member</span></span>|<span data-ttu-id="5ec65-109">值</span><span class="sxs-lookup"><span data-stu-id="5ec65-109">Value</span></span>|<span data-ttu-id="5ec65-110">说明</span><span class="sxs-lookup"><span data-stu-id="5ec65-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ec65-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="5ec65-111">deviceDefault</span></span>|<span data-ttu-id="5ec65-112">0</span><span class="sxs-lookup"><span data-stu-id="5ec65-112">0</span></span>|<span data-ttu-id="5ec65-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="5ec65-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="5ec65-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="5ec65-114">lowSecurityBiometric</span></span>|<span data-ttu-id="5ec65-115">1</span><span class="sxs-lookup"><span data-stu-id="5ec65-115">1</span></span>|<span data-ttu-id="5ec65-116">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="5ec65-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="5ec65-117">必需</span><span class="sxs-lookup"><span data-stu-id="5ec65-117">required</span></span>|<span data-ttu-id="5ec65-118">双面</span><span class="sxs-lookup"><span data-stu-id="5ec65-118">2</span></span>|<span data-ttu-id="5ec65-119">必需。</span><span class="sxs-lookup"><span data-stu-id="5ec65-119">Required.</span></span>|
|<span data-ttu-id="5ec65-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="5ec65-120">atLeastNumeric</span></span>|<span data-ttu-id="5ec65-121">第三章</span><span class="sxs-lookup"><span data-stu-id="5ec65-121">3</span></span>|<span data-ttu-id="5ec65-122">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="5ec65-122">At least numeric password required.</span></span>|
|<span data-ttu-id="5ec65-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="5ec65-123">numericComplex</span></span>|<span data-ttu-id="5ec65-124">4</span><span class="sxs-lookup"><span data-stu-id="5ec65-124">4</span></span>|<span data-ttu-id="5ec65-125">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="5ec65-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="5ec65-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="5ec65-126">atLeastAlphabetic</span></span>|<span data-ttu-id="5ec65-127">5</span><span class="sxs-lookup"><span data-stu-id="5ec65-127">5</span></span>|<span data-ttu-id="5ec65-128">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="5ec65-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="5ec65-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="5ec65-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="5ec65-130">型</span><span class="sxs-lookup"><span data-stu-id="5ec65-130">6</span></span>|<span data-ttu-id="5ec65-131">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="5ec65-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="5ec65-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="5ec65-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="5ec65-133">步</span><span class="sxs-lookup"><span data-stu-id="5ec65-133">7</span></span>|<span data-ttu-id="5ec65-134">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="5ec65-134">At least alphanumeric with symbols password required.</span></span>|





