---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e84439dbd7125d02a5413b46bca1e4e79e13089c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449244"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="415da-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="415da-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="415da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="415da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="415da-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="415da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="415da-106">Android 工作配置文件必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="415da-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="415da-107">成员</span><span class="sxs-lookup"><span data-stu-id="415da-107">Members</span></span>
|<span data-ttu-id="415da-108">成员</span><span class="sxs-lookup"><span data-stu-id="415da-108">Member</span></span>|<span data-ttu-id="415da-109">值</span><span class="sxs-lookup"><span data-stu-id="415da-109">Value</span></span>|<span data-ttu-id="415da-110">说明</span><span class="sxs-lookup"><span data-stu-id="415da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="415da-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="415da-111">deviceDefault</span></span>|<span data-ttu-id="415da-112">0</span><span class="sxs-lookup"><span data-stu-id="415da-112">0</span></span>|<span data-ttu-id="415da-113">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="415da-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="415da-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="415da-114">lowSecurityBiometric</span></span>|<span data-ttu-id="415da-115">1</span><span class="sxs-lookup"><span data-stu-id="415da-115">1</span></span>|<span data-ttu-id="415da-116">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="415da-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="415da-117">必需</span><span class="sxs-lookup"><span data-stu-id="415da-117">required</span></span>|<span data-ttu-id="415da-118">双面</span><span class="sxs-lookup"><span data-stu-id="415da-118">2</span></span>|<span data-ttu-id="415da-119">必需。</span><span class="sxs-lookup"><span data-stu-id="415da-119">Required.</span></span>|
|<span data-ttu-id="415da-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="415da-120">atLeastNumeric</span></span>|<span data-ttu-id="415da-121">第三章</span><span class="sxs-lookup"><span data-stu-id="415da-121">3</span></span>|<span data-ttu-id="415da-122">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="415da-122">At least numeric password required.</span></span>|
|<span data-ttu-id="415da-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="415da-123">numericComplex</span></span>|<span data-ttu-id="415da-124">4 </span><span class="sxs-lookup"><span data-stu-id="415da-124">4</span></span>|<span data-ttu-id="415da-125">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="415da-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="415da-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="415da-126">atLeastAlphabetic</span></span>|<span data-ttu-id="415da-127">5 </span><span class="sxs-lookup"><span data-stu-id="415da-127">5</span></span>|<span data-ttu-id="415da-128">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="415da-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="415da-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="415da-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="415da-130">6 </span><span class="sxs-lookup"><span data-stu-id="415da-130">6</span></span>|<span data-ttu-id="415da-131">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="415da-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="415da-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="415da-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="415da-133">7 </span><span class="sxs-lookup"><span data-stu-id="415da-133">7</span></span>|<span data-ttu-id="415da-134">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="415da-134">At least alphanumeric with symbols password required.</span></span>|







