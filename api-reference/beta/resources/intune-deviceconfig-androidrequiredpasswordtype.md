---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2ceac6e3953615524fb78b14c380218bf5c43f19
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796732"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="61c24-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="61c24-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="61c24-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="61c24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61c24-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61c24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61c24-106">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="61c24-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="61c24-107">成员</span><span class="sxs-lookup"><span data-stu-id="61c24-107">Members</span></span>
|<span data-ttu-id="61c24-108">成员</span><span class="sxs-lookup"><span data-stu-id="61c24-108">Member</span></span>|<span data-ttu-id="61c24-109">值</span><span class="sxs-lookup"><span data-stu-id="61c24-109">Value</span></span>|<span data-ttu-id="61c24-110">说明</span><span class="sxs-lookup"><span data-stu-id="61c24-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61c24-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="61c24-111">deviceDefault</span></span>|<span data-ttu-id="61c24-112">0</span><span class="sxs-lookup"><span data-stu-id="61c24-112">0</span></span>|<span data-ttu-id="61c24-113">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="61c24-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="61c24-114">字母</span><span class="sxs-lookup"><span data-stu-id="61c24-114">alphabetic</span></span>|<span data-ttu-id="61c24-115">1</span><span class="sxs-lookup"><span data-stu-id="61c24-115">1</span></span>|<span data-ttu-id="61c24-116">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="61c24-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="61c24-117">字母数字</span><span class="sxs-lookup"><span data-stu-id="61c24-117">alphanumeric</span></span>|<span data-ttu-id="61c24-118">双面</span><span class="sxs-lookup"><span data-stu-id="61c24-118">2</span></span>|<span data-ttu-id="61c24-119">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="61c24-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="61c24-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="61c24-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="61c24-121">第三章</span><span class="sxs-lookup"><span data-stu-id="61c24-121">3</span></span>|<span data-ttu-id="61c24-122">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="61c24-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="61c24-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="61c24-123">lowSecurityBiometric</span></span>|<span data-ttu-id="61c24-124">4 </span><span class="sxs-lookup"><span data-stu-id="61c24-124">4</span></span>|<span data-ttu-id="61c24-125">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="61c24-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="61c24-126">位数</span><span class="sxs-lookup"><span data-stu-id="61c24-126">numeric</span></span>|<span data-ttu-id="61c24-127">5 </span><span class="sxs-lookup"><span data-stu-id="61c24-127">5</span></span>|<span data-ttu-id="61c24-128">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="61c24-128">Numeric password required.</span></span>|
|<span data-ttu-id="61c24-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="61c24-129">numericComplex</span></span>|<span data-ttu-id="61c24-130">6 </span><span class="sxs-lookup"><span data-stu-id="61c24-130">6</span></span>|<span data-ttu-id="61c24-131">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="61c24-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="61c24-132">任意</span><span class="sxs-lookup"><span data-stu-id="61c24-132">any</span></span>|<span data-ttu-id="61c24-133">7 </span><span class="sxs-lookup"><span data-stu-id="61c24-133">7</span></span>|<span data-ttu-id="61c24-134">需要密码或模式，可以接受。</span><span class="sxs-lookup"><span data-stu-id="61c24-134">A password or pattern is required, and any is acceptable.</span></span>|



