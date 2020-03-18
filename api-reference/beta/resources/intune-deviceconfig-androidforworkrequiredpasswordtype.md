---
title: androidForWorkRequiredPasswordType 枚举类型
description: 适用于工作所需密码类型的 Android。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f07a89b0f7a753d15798edbe93799d2beba2f69a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796816"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="d4648-103">androidForWorkRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d4648-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="d4648-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d4648-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4648-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4648-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4648-106">适用于工作所需密码类型的 Android。</span><span class="sxs-lookup"><span data-stu-id="d4648-106">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="d4648-107">成员</span><span class="sxs-lookup"><span data-stu-id="d4648-107">Members</span></span>
|<span data-ttu-id="d4648-108">成员</span><span class="sxs-lookup"><span data-stu-id="d4648-108">Member</span></span>|<span data-ttu-id="d4648-109">值</span><span class="sxs-lookup"><span data-stu-id="d4648-109">Value</span></span>|<span data-ttu-id="d4648-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4648-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4648-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d4648-111">deviceDefault</span></span>|<span data-ttu-id="d4648-112">0</span><span class="sxs-lookup"><span data-stu-id="d4648-112">0</span></span>|<span data-ttu-id="d4648-113">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="d4648-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="d4648-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="d4648-114">lowSecurityBiometric</span></span>|<span data-ttu-id="d4648-115">1</span><span class="sxs-lookup"><span data-stu-id="d4648-115">1</span></span>|<span data-ttu-id="d4648-116">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="d4648-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="d4648-117">必需</span><span class="sxs-lookup"><span data-stu-id="d4648-117">required</span></span>|<span data-ttu-id="d4648-118">双面</span><span class="sxs-lookup"><span data-stu-id="d4648-118">2</span></span>|<span data-ttu-id="d4648-119">必需。</span><span class="sxs-lookup"><span data-stu-id="d4648-119">Required.</span></span>|
|<span data-ttu-id="d4648-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="d4648-120">atLeastNumeric</span></span>|<span data-ttu-id="d4648-121">第三章</span><span class="sxs-lookup"><span data-stu-id="d4648-121">3</span></span>|<span data-ttu-id="d4648-122">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="d4648-122">At least numeric password required.</span></span>|
|<span data-ttu-id="d4648-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="d4648-123">numericComplex</span></span>|<span data-ttu-id="d4648-124">4 </span><span class="sxs-lookup"><span data-stu-id="d4648-124">4</span></span>|<span data-ttu-id="d4648-125">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="d4648-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="d4648-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="d4648-126">atLeastAlphabetic</span></span>|<span data-ttu-id="d4648-127">5 </span><span class="sxs-lookup"><span data-stu-id="d4648-127">5</span></span>|<span data-ttu-id="d4648-128">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="d4648-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="d4648-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="d4648-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="d4648-130">6 </span><span class="sxs-lookup"><span data-stu-id="d4648-130">6</span></span>|<span data-ttu-id="d4648-131">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="d4648-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="d4648-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="d4648-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="d4648-133">7 </span><span class="sxs-lookup"><span data-stu-id="d4648-133">7</span></span>|<span data-ttu-id="d4648-134">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="d4648-134">At least alphanumeric with symbols password required.</span></span>|



