---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e20e93543ca681ebd9d900aeaac43731a3d4fa2d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444384"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="c814c-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c814c-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="c814c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c814c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c814c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c814c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c814c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c814c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c814c-107">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c814c-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="c814c-108">成员</span><span class="sxs-lookup"><span data-stu-id="c814c-108">Members</span></span>
|<span data-ttu-id="c814c-109">成员</span><span class="sxs-lookup"><span data-stu-id="c814c-109">Member</span></span>|<span data-ttu-id="c814c-110">值</span><span class="sxs-lookup"><span data-stu-id="c814c-110">Value</span></span>|<span data-ttu-id="c814c-111">说明</span><span class="sxs-lookup"><span data-stu-id="c814c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c814c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c814c-112">deviceDefault</span></span>|<span data-ttu-id="c814c-113">0</span><span class="sxs-lookup"><span data-stu-id="c814c-113">0</span></span>|<span data-ttu-id="c814c-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="c814c-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="c814c-115">字母</span><span class="sxs-lookup"><span data-stu-id="c814c-115">alphabetic</span></span>|<span data-ttu-id="c814c-116">1</span><span class="sxs-lookup"><span data-stu-id="c814c-116">1</span></span>|<span data-ttu-id="c814c-117">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="c814c-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="c814c-118">字母数字</span><span class="sxs-lookup"><span data-stu-id="c814c-118">alphanumeric</span></span>|<span data-ttu-id="c814c-119">双面</span><span class="sxs-lookup"><span data-stu-id="c814c-119">2</span></span>|<span data-ttu-id="c814c-120">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="c814c-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="c814c-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="c814c-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="c814c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="c814c-122">3</span></span>|<span data-ttu-id="c814c-123">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="c814c-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="c814c-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="c814c-124">lowSecurityBiometric</span></span>|<span data-ttu-id="c814c-125">4 </span><span class="sxs-lookup"><span data-stu-id="c814c-125">4</span></span>|<span data-ttu-id="c814c-126">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="c814c-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="c814c-127">位数</span><span class="sxs-lookup"><span data-stu-id="c814c-127">numeric</span></span>|<span data-ttu-id="c814c-128">5 </span><span class="sxs-lookup"><span data-stu-id="c814c-128">5</span></span>|<span data-ttu-id="c814c-129">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="c814c-129">Numeric password required.</span></span>|
|<span data-ttu-id="c814c-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="c814c-130">numericComplex</span></span>|<span data-ttu-id="c814c-131">6 </span><span class="sxs-lookup"><span data-stu-id="c814c-131">6</span></span>|<span data-ttu-id="c814c-132">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="c814c-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="c814c-133">任意</span><span class="sxs-lookup"><span data-stu-id="c814c-133">any</span></span>|<span data-ttu-id="c814c-134">7 </span><span class="sxs-lookup"><span data-stu-id="c814c-134">7</span></span>|<span data-ttu-id="c814c-135">需要密码或模式，可以接受。</span><span class="sxs-lookup"><span data-stu-id="c814c-135">A password or pattern is required, and any is acceptable.</span></span>|



