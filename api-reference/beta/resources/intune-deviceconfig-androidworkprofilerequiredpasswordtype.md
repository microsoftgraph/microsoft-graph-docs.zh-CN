---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 865f867510df85b3f784930558bad948c26d5d61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527194"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="54df2-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="54df2-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="54df2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="54df2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54df2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="54df2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54df2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54df2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54df2-107">Android 工作配置文件必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="54df2-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="54df2-108">成员</span><span class="sxs-lookup"><span data-stu-id="54df2-108">Members</span></span>
|<span data-ttu-id="54df2-109">成员</span><span class="sxs-lookup"><span data-stu-id="54df2-109">Member</span></span>|<span data-ttu-id="54df2-110">值</span><span class="sxs-lookup"><span data-stu-id="54df2-110">Value</span></span>|<span data-ttu-id="54df2-111">说明</span><span class="sxs-lookup"><span data-stu-id="54df2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54df2-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="54df2-112">deviceDefault</span></span>|<span data-ttu-id="54df2-113">0</span><span class="sxs-lookup"><span data-stu-id="54df2-113">0</span></span>|<span data-ttu-id="54df2-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="54df2-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="54df2-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="54df2-115">lowSecurityBiometric</span></span>|<span data-ttu-id="54df2-116">1 </span><span class="sxs-lookup"><span data-stu-id="54df2-116">1</span></span>|<span data-ttu-id="54df2-117">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="54df2-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="54df2-118">必需</span><span class="sxs-lookup"><span data-stu-id="54df2-118">required</span></span>|<span data-ttu-id="54df2-119">2 </span><span class="sxs-lookup"><span data-stu-id="54df2-119">2</span></span>|<span data-ttu-id="54df2-120">必填。</span><span class="sxs-lookup"><span data-stu-id="54df2-120">Required.</span></span>|
|<span data-ttu-id="54df2-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="54df2-121">atLeastNumeric</span></span>|<span data-ttu-id="54df2-122">3 </span><span class="sxs-lookup"><span data-stu-id="54df2-122">3</span></span>|<span data-ttu-id="54df2-123">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="54df2-123">At least numeric password required.</span></span>|
|<span data-ttu-id="54df2-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="54df2-124">numericComplex</span></span>|<span data-ttu-id="54df2-125">4 </span><span class="sxs-lookup"><span data-stu-id="54df2-125">4</span></span>|<span data-ttu-id="54df2-126">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="54df2-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="54df2-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="54df2-127">atLeastAlphabetic</span></span>|<span data-ttu-id="54df2-128">5 </span><span class="sxs-lookup"><span data-stu-id="54df2-128">5</span></span>|<span data-ttu-id="54df2-129">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="54df2-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="54df2-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="54df2-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="54df2-131">6 </span><span class="sxs-lookup"><span data-stu-id="54df2-131">6</span></span>|<span data-ttu-id="54df2-132">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="54df2-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="54df2-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="54df2-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="54df2-134">7 </span><span class="sxs-lookup"><span data-stu-id="54df2-134">7</span></span>|<span data-ttu-id="54df2-135">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="54df2-135">At least alphanumeric with symbols password required.</span></span>|



