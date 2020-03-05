---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7d20aee3893d9d74e01fad6858c59d2c524059d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527304"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="7a8f6-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7a8f6-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="7a8f6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7a8f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a8f6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7a8f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a8f6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a8f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a8f6-107">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="7a8f6-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="7a8f6-108">成员</span><span class="sxs-lookup"><span data-stu-id="7a8f6-108">Members</span></span>
|<span data-ttu-id="7a8f6-109">成员</span><span class="sxs-lookup"><span data-stu-id="7a8f6-109">Member</span></span>|<span data-ttu-id="7a8f6-110">值</span><span class="sxs-lookup"><span data-stu-id="7a8f6-110">Value</span></span>|<span data-ttu-id="7a8f6-111">说明</span><span class="sxs-lookup"><span data-stu-id="7a8f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a8f6-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7a8f6-112">deviceDefault</span></span>|<span data-ttu-id="7a8f6-113">0</span><span class="sxs-lookup"><span data-stu-id="7a8f6-113">0</span></span>|<span data-ttu-id="7a8f6-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="7a8f6-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="7a8f6-115">字母</span><span class="sxs-lookup"><span data-stu-id="7a8f6-115">alphabetic</span></span>|<span data-ttu-id="7a8f6-116">1 </span><span class="sxs-lookup"><span data-stu-id="7a8f6-116">1</span></span>|<span data-ttu-id="7a8f6-117">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="7a8f6-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="7a8f6-118">字母数字</span><span class="sxs-lookup"><span data-stu-id="7a8f6-118">alphanumeric</span></span>|<span data-ttu-id="7a8f6-119">2 </span><span class="sxs-lookup"><span data-stu-id="7a8f6-119">2</span></span>|<span data-ttu-id="7a8f6-120">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="7a8f6-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="7a8f6-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="7a8f6-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="7a8f6-122">3 </span><span class="sxs-lookup"><span data-stu-id="7a8f6-122">3</span></span>|<span data-ttu-id="7a8f6-123">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="7a8f6-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="7a8f6-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="7a8f6-124">lowSecurityBiometric</span></span>|<span data-ttu-id="7a8f6-125">4 </span><span class="sxs-lookup"><span data-stu-id="7a8f6-125">4</span></span>|<span data-ttu-id="7a8f6-126">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="7a8f6-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="7a8f6-127">位数</span><span class="sxs-lookup"><span data-stu-id="7a8f6-127">numeric</span></span>|<span data-ttu-id="7a8f6-128">5 </span><span class="sxs-lookup"><span data-stu-id="7a8f6-128">5</span></span>|<span data-ttu-id="7a8f6-129">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="7a8f6-129">Numeric password required.</span></span>|
|<span data-ttu-id="7a8f6-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="7a8f6-130">numericComplex</span></span>|<span data-ttu-id="7a8f6-131">6 </span><span class="sxs-lookup"><span data-stu-id="7a8f6-131">6</span></span>|<span data-ttu-id="7a8f6-132">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="7a8f6-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="7a8f6-133">任意</span><span class="sxs-lookup"><span data-stu-id="7a8f6-133">any</span></span>|<span data-ttu-id="7a8f6-134">7 </span><span class="sxs-lookup"><span data-stu-id="7a8f6-134">7</span></span>|<span data-ttu-id="7a8f6-135">需要密码或模式，可以接受。</span><span class="sxs-lookup"><span data-stu-id="7a8f6-135">A password or pattern is required, and any is acceptable.</span></span>|



