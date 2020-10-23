---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f78829f47a8f1d029ed78b2fb0d63192af69a3e6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725601"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="3d4c9-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3d4c9-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="3d4c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d4c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d4c9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d4c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d4c9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d4c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d4c9-107">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="3d4c9-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="3d4c9-108">成员</span><span class="sxs-lookup"><span data-stu-id="3d4c9-108">Members</span></span>
|<span data-ttu-id="3d4c9-109">成员</span><span class="sxs-lookup"><span data-stu-id="3d4c9-109">Member</span></span>|<span data-ttu-id="3d4c9-110">值</span><span class="sxs-lookup"><span data-stu-id="3d4c9-110">Value</span></span>|<span data-ttu-id="3d4c9-111">说明</span><span class="sxs-lookup"><span data-stu-id="3d4c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d4c9-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3d4c9-112">deviceDefault</span></span>|<span data-ttu-id="3d4c9-113">0</span><span class="sxs-lookup"><span data-stu-id="3d4c9-113">0</span></span>|<span data-ttu-id="3d4c9-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="3d4c9-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="3d4c9-115">字母</span><span class="sxs-lookup"><span data-stu-id="3d4c9-115">alphabetic</span></span>|<span data-ttu-id="3d4c9-116">1</span><span class="sxs-lookup"><span data-stu-id="3d4c9-116">1</span></span>|<span data-ttu-id="3d4c9-117">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="3d4c9-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="3d4c9-118">字母数字</span><span class="sxs-lookup"><span data-stu-id="3d4c9-118">alphanumeric</span></span>|<span data-ttu-id="3d4c9-119">双面</span><span class="sxs-lookup"><span data-stu-id="3d4c9-119">2</span></span>|<span data-ttu-id="3d4c9-120">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="3d4c9-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="3d4c9-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="3d4c9-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="3d4c9-122">第三章</span><span class="sxs-lookup"><span data-stu-id="3d4c9-122">3</span></span>|<span data-ttu-id="3d4c9-123">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="3d4c9-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="3d4c9-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="3d4c9-124">lowSecurityBiometric</span></span>|<span data-ttu-id="3d4c9-125">4 </span><span class="sxs-lookup"><span data-stu-id="3d4c9-125">4</span></span>|<span data-ttu-id="3d4c9-126">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="3d4c9-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="3d4c9-127">位数</span><span class="sxs-lookup"><span data-stu-id="3d4c9-127">numeric</span></span>|<span data-ttu-id="3d4c9-128">5 </span><span class="sxs-lookup"><span data-stu-id="3d4c9-128">5</span></span>|<span data-ttu-id="3d4c9-129">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="3d4c9-129">Numeric password required.</span></span>|
|<span data-ttu-id="3d4c9-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="3d4c9-130">numericComplex</span></span>|<span data-ttu-id="3d4c9-131">6 </span><span class="sxs-lookup"><span data-stu-id="3d4c9-131">6</span></span>|<span data-ttu-id="3d4c9-132">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="3d4c9-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="3d4c9-133">任意</span><span class="sxs-lookup"><span data-stu-id="3d4c9-133">any</span></span>|<span data-ttu-id="3d4c9-134">7 </span><span class="sxs-lookup"><span data-stu-id="3d4c9-134">7</span></span>|<span data-ttu-id="3d4c9-135">需要密码或模式，可以接受。</span><span class="sxs-lookup"><span data-stu-id="3d4c9-135">A password or pattern is required, and any is acceptable.</span></span>|





