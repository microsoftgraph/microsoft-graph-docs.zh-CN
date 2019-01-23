---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eebc6b0ad6eed346927fd48a2dc1f82b5e529b28
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392911"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="6639e-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6639e-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="6639e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6639e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6639e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6639e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6639e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6639e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6639e-107">Android 所需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="6639e-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="6639e-108">成员</span><span class="sxs-lookup"><span data-stu-id="6639e-108">Members</span></span>
|<span data-ttu-id="6639e-109">成员</span><span class="sxs-lookup"><span data-stu-id="6639e-109">Member</span></span>|<span data-ttu-id="6639e-110">值</span><span class="sxs-lookup"><span data-stu-id="6639e-110">Value</span></span>|<span data-ttu-id="6639e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6639e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6639e-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="6639e-112">deviceDefault</span></span>|<span data-ttu-id="6639e-113">0</span><span class="sxs-lookup"><span data-stu-id="6639e-113">0</span></span>|<span data-ttu-id="6639e-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="6639e-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="6639e-115">字母</span><span class="sxs-lookup"><span data-stu-id="6639e-115">alphabetic</span></span>|<span data-ttu-id="6639e-116">1</span><span class="sxs-lookup"><span data-stu-id="6639e-116">1</span></span>|<span data-ttu-id="6639e-117">所需的密码字母。</span><span class="sxs-lookup"><span data-stu-id="6639e-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="6639e-118">字母数字</span><span class="sxs-lookup"><span data-stu-id="6639e-118">alphanumeric</span></span>|<span data-ttu-id="6639e-119">2</span><span class="sxs-lookup"><span data-stu-id="6639e-119">2</span></span>|<span data-ttu-id="6639e-120">所需的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="6639e-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="6639e-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="6639e-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="6639e-122">3</span><span class="sxs-lookup"><span data-stu-id="6639e-122">3</span></span>|<span data-ttu-id="6639e-123">所需的符号密码全角字母数字。</span><span class="sxs-lookup"><span data-stu-id="6639e-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="6639e-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="6639e-124">lowSecurityBiometric</span></span>|<span data-ttu-id="6639e-125">4</span><span class="sxs-lookup"><span data-stu-id="6639e-125">4</span></span>|<span data-ttu-id="6639e-126">低安全性生物基于所需的密码。</span><span class="sxs-lookup"><span data-stu-id="6639e-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="6639e-127">数值</span><span class="sxs-lookup"><span data-stu-id="6639e-127">numeric</span></span>|<span data-ttu-id="6639e-128">5</span><span class="sxs-lookup"><span data-stu-id="6639e-128">5</span></span>|<span data-ttu-id="6639e-129">所需的数字密码。</span><span class="sxs-lookup"><span data-stu-id="6639e-129">Numeric password required.</span></span>|
|<span data-ttu-id="6639e-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="6639e-130">numericComplex</span></span>|<span data-ttu-id="6639e-131">6</span><span class="sxs-lookup"><span data-stu-id="6639e-131">6</span></span>|<span data-ttu-id="6639e-132">所需的数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="6639e-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="6639e-133">任意</span><span class="sxs-lookup"><span data-stu-id="6639e-133">any</span></span>|<span data-ttu-id="6639e-134">7</span><span class="sxs-lookup"><span data-stu-id="6639e-134">7</span></span>|<span data-ttu-id="6639e-135">Password 或模式是必需的且任何可接受。</span><span class="sxs-lookup"><span data-stu-id="6639e-135">A password or pattern is required, and any is acceptable.</span></span>|




