---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件所需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 741a86f1ce4654fe6d5495521f055490d4c068bc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755943"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="be2b0-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="be2b0-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="be2b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be2b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be2b0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be2b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be2b0-106">Android 工作配置文件所需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="be2b0-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="be2b0-107">成员</span><span class="sxs-lookup"><span data-stu-id="be2b0-107">Members</span></span>
|<span data-ttu-id="be2b0-108">成员</span><span class="sxs-lookup"><span data-stu-id="be2b0-108">Member</span></span>|<span data-ttu-id="be2b0-109">值</span><span class="sxs-lookup"><span data-stu-id="be2b0-109">Value</span></span>|<span data-ttu-id="be2b0-110">说明</span><span class="sxs-lookup"><span data-stu-id="be2b0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be2b0-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="be2b0-111">deviceDefault</span></span>|<span data-ttu-id="be2b0-112">0</span><span class="sxs-lookup"><span data-stu-id="be2b0-112">0</span></span>|<span data-ttu-id="be2b0-113">设备默认值，无意图。</span><span class="sxs-lookup"><span data-stu-id="be2b0-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="be2b0-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="be2b0-114">lowSecurityBiometric</span></span>|<span data-ttu-id="be2b0-115">1</span><span class="sxs-lookup"><span data-stu-id="be2b0-115">1</span></span>|<span data-ttu-id="be2b0-116">需要低安全生物识别密码。</span><span class="sxs-lookup"><span data-stu-id="be2b0-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="be2b0-117">必需</span><span class="sxs-lookup"><span data-stu-id="be2b0-117">required</span></span>|<span data-ttu-id="be2b0-118">2</span><span class="sxs-lookup"><span data-stu-id="be2b0-118">2</span></span>|<span data-ttu-id="be2b0-119">必填。</span><span class="sxs-lookup"><span data-stu-id="be2b0-119">Required.</span></span>|
|<span data-ttu-id="be2b0-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="be2b0-120">atLeastNumeric</span></span>|<span data-ttu-id="be2b0-121">3</span><span class="sxs-lookup"><span data-stu-id="be2b0-121">3</span></span>|<span data-ttu-id="be2b0-122">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="be2b0-122">At least numeric password required.</span></span>|
|<span data-ttu-id="be2b0-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="be2b0-123">numericComplex</span></span>|<span data-ttu-id="be2b0-124">4 </span><span class="sxs-lookup"><span data-stu-id="be2b0-124">4</span></span>|<span data-ttu-id="be2b0-125">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="be2b0-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="be2b0-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="be2b0-126">atLeastAlphabetic</span></span>|<span data-ttu-id="be2b0-127">5 </span><span class="sxs-lookup"><span data-stu-id="be2b0-127">5</span></span>|<span data-ttu-id="be2b0-128">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="be2b0-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="be2b0-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="be2b0-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="be2b0-130">6 </span><span class="sxs-lookup"><span data-stu-id="be2b0-130">6</span></span>|<span data-ttu-id="be2b0-131">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="be2b0-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="be2b0-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="be2b0-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="be2b0-133">7 </span><span class="sxs-lookup"><span data-stu-id="be2b0-133">7</span></span>|<span data-ttu-id="be2b0-134">至少包含需要符号密码的字母数字。</span><span class="sxs-lookup"><span data-stu-id="be2b0-134">At least alphanumeric with symbols password required.</span></span>|




