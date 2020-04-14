---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b3c2b0945d91bead7f28ec49e53c68f89fbb19d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470220"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="42379-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="42379-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="42379-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42379-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42379-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42379-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42379-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42379-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42379-107">Android 工作配置文件必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="42379-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="42379-108">成员</span><span class="sxs-lookup"><span data-stu-id="42379-108">Members</span></span>
|<span data-ttu-id="42379-109">成员</span><span class="sxs-lookup"><span data-stu-id="42379-109">Member</span></span>|<span data-ttu-id="42379-110">值</span><span class="sxs-lookup"><span data-stu-id="42379-110">Value</span></span>|<span data-ttu-id="42379-111">说明</span><span class="sxs-lookup"><span data-stu-id="42379-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42379-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="42379-112">deviceDefault</span></span>|<span data-ttu-id="42379-113">0</span><span class="sxs-lookup"><span data-stu-id="42379-113">0</span></span>|<span data-ttu-id="42379-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="42379-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="42379-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="42379-115">lowSecurityBiometric</span></span>|<span data-ttu-id="42379-116">1</span><span class="sxs-lookup"><span data-stu-id="42379-116">1</span></span>|<span data-ttu-id="42379-117">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="42379-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="42379-118">必需</span><span class="sxs-lookup"><span data-stu-id="42379-118">required</span></span>|<span data-ttu-id="42379-119">双面</span><span class="sxs-lookup"><span data-stu-id="42379-119">2</span></span>|<span data-ttu-id="42379-120">必需。</span><span class="sxs-lookup"><span data-stu-id="42379-120">Required.</span></span>|
|<span data-ttu-id="42379-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="42379-121">atLeastNumeric</span></span>|<span data-ttu-id="42379-122">第三章</span><span class="sxs-lookup"><span data-stu-id="42379-122">3</span></span>|<span data-ttu-id="42379-123">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="42379-123">At least numeric password required.</span></span>|
|<span data-ttu-id="42379-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="42379-124">numericComplex</span></span>|<span data-ttu-id="42379-125">4 </span><span class="sxs-lookup"><span data-stu-id="42379-125">4</span></span>|<span data-ttu-id="42379-126">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="42379-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="42379-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="42379-127">atLeastAlphabetic</span></span>|<span data-ttu-id="42379-128">5 </span><span class="sxs-lookup"><span data-stu-id="42379-128">5</span></span>|<span data-ttu-id="42379-129">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="42379-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="42379-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="42379-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="42379-131">6 </span><span class="sxs-lookup"><span data-stu-id="42379-131">6</span></span>|<span data-ttu-id="42379-132">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="42379-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="42379-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="42379-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="42379-134">7 </span><span class="sxs-lookup"><span data-stu-id="42379-134">7</span></span>|<span data-ttu-id="42379-135">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="42379-135">At least alphanumeric with symbols password required.</span></span>|



