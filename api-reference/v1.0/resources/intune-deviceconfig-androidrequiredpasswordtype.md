---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4921263e1960617b8d9e013ce12a799e11d61516
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041559"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="2154a-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2154a-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="2154a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2154a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2154a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2154a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2154a-106">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="2154a-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="2154a-107">成员</span><span class="sxs-lookup"><span data-stu-id="2154a-107">Members</span></span>
|<span data-ttu-id="2154a-108">成员</span><span class="sxs-lookup"><span data-stu-id="2154a-108">Member</span></span>|<span data-ttu-id="2154a-109">值</span><span class="sxs-lookup"><span data-stu-id="2154a-109">Value</span></span>|<span data-ttu-id="2154a-110">说明</span><span class="sxs-lookup"><span data-stu-id="2154a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2154a-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="2154a-111">deviceDefault</span></span>|<span data-ttu-id="2154a-112">0</span><span class="sxs-lookup"><span data-stu-id="2154a-112">0</span></span>|<span data-ttu-id="2154a-113">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="2154a-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="2154a-114">字母</span><span class="sxs-lookup"><span data-stu-id="2154a-114">alphabetic</span></span>|<span data-ttu-id="2154a-115">1 </span><span class="sxs-lookup"><span data-stu-id="2154a-115">1</span></span>|<span data-ttu-id="2154a-116">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="2154a-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="2154a-117">字母数字</span><span class="sxs-lookup"><span data-stu-id="2154a-117">alphanumeric</span></span>|<span data-ttu-id="2154a-118">2 </span><span class="sxs-lookup"><span data-stu-id="2154a-118">2</span></span>|<span data-ttu-id="2154a-119">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="2154a-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="2154a-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="2154a-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="2154a-121">第三章</span><span class="sxs-lookup"><span data-stu-id="2154a-121">3</span></span>|<span data-ttu-id="2154a-122">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="2154a-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="2154a-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="2154a-123">lowSecurityBiometric</span></span>|<span data-ttu-id="2154a-124">4 </span><span class="sxs-lookup"><span data-stu-id="2154a-124">4</span></span>|<span data-ttu-id="2154a-125">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="2154a-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="2154a-126">位数</span><span class="sxs-lookup"><span data-stu-id="2154a-126">numeric</span></span>|<span data-ttu-id="2154a-127">5 </span><span class="sxs-lookup"><span data-stu-id="2154a-127">5</span></span>|<span data-ttu-id="2154a-128">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="2154a-128">Numeric password required.</span></span>|
|<span data-ttu-id="2154a-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="2154a-129">numericComplex</span></span>|<span data-ttu-id="2154a-130">6 </span><span class="sxs-lookup"><span data-stu-id="2154a-130">6</span></span>|<span data-ttu-id="2154a-131">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="2154a-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="2154a-132">任意</span><span class="sxs-lookup"><span data-stu-id="2154a-132">any</span></span>|<span data-ttu-id="2154a-133">7 </span><span class="sxs-lookup"><span data-stu-id="2154a-133">7</span></span>|<span data-ttu-id="2154a-134">需要密码或模式，可以接受。</span><span class="sxs-lookup"><span data-stu-id="2154a-134">A password or pattern is required, and any is acceptable.</span></span>|









