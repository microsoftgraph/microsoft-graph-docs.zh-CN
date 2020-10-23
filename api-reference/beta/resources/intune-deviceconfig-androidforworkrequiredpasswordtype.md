---
title: androidForWorkRequiredPasswordType 枚举类型
description: 适用于工作所需密码类型的 Android。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 249a5081e63bd94885bdee059ae1521e03c52e71
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724626"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="945e1-103">androidForWorkRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="945e1-103">androidForWorkRequiredPasswordType enum type</span></span>

<span data-ttu-id="945e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="945e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="945e1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="945e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="945e1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="945e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="945e1-107">适用于工作所需密码类型的 Android。</span><span class="sxs-lookup"><span data-stu-id="945e1-107">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="945e1-108">成员</span><span class="sxs-lookup"><span data-stu-id="945e1-108">Members</span></span>
|<span data-ttu-id="945e1-109">成员</span><span class="sxs-lookup"><span data-stu-id="945e1-109">Member</span></span>|<span data-ttu-id="945e1-110">值</span><span class="sxs-lookup"><span data-stu-id="945e1-110">Value</span></span>|<span data-ttu-id="945e1-111">说明</span><span class="sxs-lookup"><span data-stu-id="945e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="945e1-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="945e1-112">deviceDefault</span></span>|<span data-ttu-id="945e1-113">0</span><span class="sxs-lookup"><span data-stu-id="945e1-113">0</span></span>|<span data-ttu-id="945e1-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="945e1-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="945e1-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="945e1-115">lowSecurityBiometric</span></span>|<span data-ttu-id="945e1-116">1</span><span class="sxs-lookup"><span data-stu-id="945e1-116">1</span></span>|<span data-ttu-id="945e1-117">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="945e1-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="945e1-118">必需</span><span class="sxs-lookup"><span data-stu-id="945e1-118">required</span></span>|<span data-ttu-id="945e1-119">双面</span><span class="sxs-lookup"><span data-stu-id="945e1-119">2</span></span>|<span data-ttu-id="945e1-120">必需。</span><span class="sxs-lookup"><span data-stu-id="945e1-120">Required.</span></span>|
|<span data-ttu-id="945e1-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="945e1-121">atLeastNumeric</span></span>|<span data-ttu-id="945e1-122">第三章</span><span class="sxs-lookup"><span data-stu-id="945e1-122">3</span></span>|<span data-ttu-id="945e1-123">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="945e1-123">At least numeric password required.</span></span>|
|<span data-ttu-id="945e1-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="945e1-124">numericComplex</span></span>|<span data-ttu-id="945e1-125">4 </span><span class="sxs-lookup"><span data-stu-id="945e1-125">4</span></span>|<span data-ttu-id="945e1-126">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="945e1-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="945e1-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="945e1-127">atLeastAlphabetic</span></span>|<span data-ttu-id="945e1-128">5 </span><span class="sxs-lookup"><span data-stu-id="945e1-128">5</span></span>|<span data-ttu-id="945e1-129">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="945e1-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="945e1-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="945e1-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="945e1-131">6 </span><span class="sxs-lookup"><span data-stu-id="945e1-131">6</span></span>|<span data-ttu-id="945e1-132">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="945e1-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="945e1-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="945e1-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="945e1-134">7 </span><span class="sxs-lookup"><span data-stu-id="945e1-134">7</span></span>|<span data-ttu-id="945e1-135">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="945e1-135">At least alphanumeric with symbols password required.</span></span>|





