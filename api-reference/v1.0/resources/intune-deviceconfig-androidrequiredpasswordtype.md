---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0562d059ca69358190c49fb6b518abccdc98c449
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028705"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="d9c86-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d9c86-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="d9c86-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9c86-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9c86-105">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="d9c86-105">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="d9c86-106">成员</span><span class="sxs-lookup"><span data-stu-id="d9c86-106">Members</span></span>
|<span data-ttu-id="d9c86-107">成员</span><span class="sxs-lookup"><span data-stu-id="d9c86-107">Member</span></span>|<span data-ttu-id="d9c86-108">值</span><span class="sxs-lookup"><span data-stu-id="d9c86-108">Value</span></span>|<span data-ttu-id="d9c86-109">说明</span><span class="sxs-lookup"><span data-stu-id="d9c86-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9c86-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d9c86-110">deviceDefault</span></span>|<span data-ttu-id="d9c86-111">0</span><span class="sxs-lookup"><span data-stu-id="d9c86-111">0</span></span>|<span data-ttu-id="d9c86-112">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="d9c86-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="d9c86-113">字母</span><span class="sxs-lookup"><span data-stu-id="d9c86-113">alphabetic</span></span>|<span data-ttu-id="d9c86-114">1</span><span class="sxs-lookup"><span data-stu-id="d9c86-114">1</span></span>|<span data-ttu-id="d9c86-115">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="d9c86-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="d9c86-116">字母数字</span><span class="sxs-lookup"><span data-stu-id="d9c86-116">alphanumeric</span></span>|<span data-ttu-id="d9c86-117">双面</span><span class="sxs-lookup"><span data-stu-id="d9c86-117">2</span></span>|<span data-ttu-id="d9c86-118">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="d9c86-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="d9c86-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="d9c86-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="d9c86-120">第三章</span><span class="sxs-lookup"><span data-stu-id="d9c86-120">3</span></span>|<span data-ttu-id="d9c86-121">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="d9c86-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="d9c86-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="d9c86-122">lowSecurityBiometric</span></span>|<span data-ttu-id="d9c86-123">4</span><span class="sxs-lookup"><span data-stu-id="d9c86-123">4</span></span>|<span data-ttu-id="d9c86-124">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="d9c86-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="d9c86-125">位数</span><span class="sxs-lookup"><span data-stu-id="d9c86-125">numeric</span></span>|<span data-ttu-id="d9c86-126">5</span><span class="sxs-lookup"><span data-stu-id="d9c86-126">5</span></span>|<span data-ttu-id="d9c86-127">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="d9c86-127">Numeric password required.</span></span>|
|<span data-ttu-id="d9c86-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="d9c86-128">numericComplex</span></span>|<span data-ttu-id="d9c86-129">型</span><span class="sxs-lookup"><span data-stu-id="d9c86-129">6</span></span>|<span data-ttu-id="d9c86-130">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="d9c86-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="d9c86-131">任意</span><span class="sxs-lookup"><span data-stu-id="d9c86-131">any</span></span>|<span data-ttu-id="d9c86-132">步</span><span class="sxs-lookup"><span data-stu-id="d9c86-132">7</span></span>|<span data-ttu-id="d9c86-133">需要密码或模式, 可以接受。</span><span class="sxs-lookup"><span data-stu-id="d9c86-133">A password or pattern is required, and any is acceptable.</span></span>|



