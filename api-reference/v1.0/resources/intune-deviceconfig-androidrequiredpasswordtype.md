---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59a95c74f19fa6e14440eaedd06d385b05d81e5d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575168"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="41ae5-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="41ae5-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="41ae5-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41ae5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41ae5-105">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="41ae5-105">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="41ae5-106">成员</span><span class="sxs-lookup"><span data-stu-id="41ae5-106">Members</span></span>
|<span data-ttu-id="41ae5-107">成员</span><span class="sxs-lookup"><span data-stu-id="41ae5-107">Member</span></span>|<span data-ttu-id="41ae5-108">值</span><span class="sxs-lookup"><span data-stu-id="41ae5-108">Value</span></span>|<span data-ttu-id="41ae5-109">说明</span><span class="sxs-lookup"><span data-stu-id="41ae5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41ae5-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="41ae5-110">deviceDefault</span></span>|<span data-ttu-id="41ae5-111">0</span><span class="sxs-lookup"><span data-stu-id="41ae5-111">0</span></span>|<span data-ttu-id="41ae5-112">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="41ae5-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="41ae5-113">字母</span><span class="sxs-lookup"><span data-stu-id="41ae5-113">alphabetic</span></span>|<span data-ttu-id="41ae5-114">1</span><span class="sxs-lookup"><span data-stu-id="41ae5-114">1</span></span>|<span data-ttu-id="41ae5-115">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="41ae5-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="41ae5-116">字母数字</span><span class="sxs-lookup"><span data-stu-id="41ae5-116">alphanumeric</span></span>|<span data-ttu-id="41ae5-117">2 </span><span class="sxs-lookup"><span data-stu-id="41ae5-117">2</span></span>|<span data-ttu-id="41ae5-118">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="41ae5-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="41ae5-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="41ae5-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="41ae5-120">3 </span><span class="sxs-lookup"><span data-stu-id="41ae5-120">3</span></span>|<span data-ttu-id="41ae5-121">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="41ae5-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="41ae5-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="41ae5-122">lowSecurityBiometric</span></span>|<span data-ttu-id="41ae5-123">4 </span><span class="sxs-lookup"><span data-stu-id="41ae5-123">4</span></span>|<span data-ttu-id="41ae5-124">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="41ae5-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="41ae5-125">位数</span><span class="sxs-lookup"><span data-stu-id="41ae5-125">numeric</span></span>|<span data-ttu-id="41ae5-126">5 </span><span class="sxs-lookup"><span data-stu-id="41ae5-126">5</span></span>|<span data-ttu-id="41ae5-127">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="41ae5-127">Numeric password required.</span></span>|
|<span data-ttu-id="41ae5-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="41ae5-128">numericComplex</span></span>|<span data-ttu-id="41ae5-129">6 </span><span class="sxs-lookup"><span data-stu-id="41ae5-129">6</span></span>|<span data-ttu-id="41ae5-130">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="41ae5-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="41ae5-131">任意</span><span class="sxs-lookup"><span data-stu-id="41ae5-131">any</span></span>|<span data-ttu-id="41ae5-132">7 </span><span class="sxs-lookup"><span data-stu-id="41ae5-132">7</span></span>|<span data-ttu-id="41ae5-133">需要密码或模式, 可以接受。</span><span class="sxs-lookup"><span data-stu-id="41ae5-133">A password or pattern is required, and any is acceptable.</span></span>|



