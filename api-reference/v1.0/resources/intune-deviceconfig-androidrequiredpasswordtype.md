---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d179666a4de9256e98c704bccd9e512d4aebd0ce
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760284"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="a6f57-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a6f57-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="a6f57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6f57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6f57-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6f57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6f57-106">Android 所需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="a6f57-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="a6f57-107">成员</span><span class="sxs-lookup"><span data-stu-id="a6f57-107">Members</span></span>
|<span data-ttu-id="a6f57-108">成员</span><span class="sxs-lookup"><span data-stu-id="a6f57-108">Member</span></span>|<span data-ttu-id="a6f57-109">值</span><span class="sxs-lookup"><span data-stu-id="a6f57-109">Value</span></span>|<span data-ttu-id="a6f57-110">说明</span><span class="sxs-lookup"><span data-stu-id="a6f57-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6f57-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a6f57-111">deviceDefault</span></span>|<span data-ttu-id="a6f57-112">0</span><span class="sxs-lookup"><span data-stu-id="a6f57-112">0</span></span>|<span data-ttu-id="a6f57-113">设备默认值，无意图。</span><span class="sxs-lookup"><span data-stu-id="a6f57-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="a6f57-114">字母</span><span class="sxs-lookup"><span data-stu-id="a6f57-114">alphabetic</span></span>|<span data-ttu-id="a6f57-115">1</span><span class="sxs-lookup"><span data-stu-id="a6f57-115">1</span></span>|<span data-ttu-id="a6f57-116">需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="a6f57-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="a6f57-117">alphanumeric</span><span class="sxs-lookup"><span data-stu-id="a6f57-117">alphanumeric</span></span>|<span data-ttu-id="a6f57-118">2</span><span class="sxs-lookup"><span data-stu-id="a6f57-118">2</span></span>|<span data-ttu-id="a6f57-119">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="a6f57-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="a6f57-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="a6f57-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="a6f57-121">3</span><span class="sxs-lookup"><span data-stu-id="a6f57-121">3</span></span>|<span data-ttu-id="a6f57-122">需要符号密码的字母数字。</span><span class="sxs-lookup"><span data-stu-id="a6f57-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="a6f57-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="a6f57-123">lowSecurityBiometric</span></span>|<span data-ttu-id="a6f57-124">4 </span><span class="sxs-lookup"><span data-stu-id="a6f57-124">4</span></span>|<span data-ttu-id="a6f57-125">需要低安全生物识别密码。</span><span class="sxs-lookup"><span data-stu-id="a6f57-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="a6f57-126">numeric</span><span class="sxs-lookup"><span data-stu-id="a6f57-126">numeric</span></span>|<span data-ttu-id="a6f57-127">5 </span><span class="sxs-lookup"><span data-stu-id="a6f57-127">5</span></span>|<span data-ttu-id="a6f57-128">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="a6f57-128">Numeric password required.</span></span>|
|<span data-ttu-id="a6f57-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="a6f57-129">numericComplex</span></span>|<span data-ttu-id="a6f57-130">6 </span><span class="sxs-lookup"><span data-stu-id="a6f57-130">6</span></span>|<span data-ttu-id="a6f57-131">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="a6f57-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="a6f57-132">任意</span><span class="sxs-lookup"><span data-stu-id="a6f57-132">any</span></span>|<span data-ttu-id="a6f57-133">7 </span><span class="sxs-lookup"><span data-stu-id="a6f57-133">7</span></span>|<span data-ttu-id="a6f57-134">密码或模式是必需的，任何密码或模式都是可接受的。</span><span class="sxs-lookup"><span data-stu-id="a6f57-134">A password or pattern is required, and any is acceptable.</span></span>|




