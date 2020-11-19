---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: aa7ab836addd205d0b39c14fa0dcb42dd71bb81a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256958"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="110b9-103">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="110b9-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="110b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="110b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="110b9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="110b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="110b9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="110b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="110b9-107">Android 工作配置文件必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="110b9-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="110b9-108">成员</span><span class="sxs-lookup"><span data-stu-id="110b9-108">Members</span></span>
|<span data-ttu-id="110b9-109">成员</span><span class="sxs-lookup"><span data-stu-id="110b9-109">Member</span></span>|<span data-ttu-id="110b9-110">值</span><span class="sxs-lookup"><span data-stu-id="110b9-110">Value</span></span>|<span data-ttu-id="110b9-111">说明</span><span class="sxs-lookup"><span data-stu-id="110b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="110b9-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="110b9-112">deviceDefault</span></span>|<span data-ttu-id="110b9-113">0</span><span class="sxs-lookup"><span data-stu-id="110b9-113">0</span></span>|<span data-ttu-id="110b9-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="110b9-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="110b9-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="110b9-115">lowSecurityBiometric</span></span>|<span data-ttu-id="110b9-116">1</span><span class="sxs-lookup"><span data-stu-id="110b9-116">1</span></span>|<span data-ttu-id="110b9-117">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="110b9-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="110b9-118">必需</span><span class="sxs-lookup"><span data-stu-id="110b9-118">required</span></span>|<span data-ttu-id="110b9-119">双面</span><span class="sxs-lookup"><span data-stu-id="110b9-119">2</span></span>|<span data-ttu-id="110b9-120">必需。</span><span class="sxs-lookup"><span data-stu-id="110b9-120">Required.</span></span>|
|<span data-ttu-id="110b9-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="110b9-121">atLeastNumeric</span></span>|<span data-ttu-id="110b9-122">第三章</span><span class="sxs-lookup"><span data-stu-id="110b9-122">3</span></span>|<span data-ttu-id="110b9-123">至少需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="110b9-123">At least numeric password required.</span></span>|
|<span data-ttu-id="110b9-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="110b9-124">numericComplex</span></span>|<span data-ttu-id="110b9-125">4 </span><span class="sxs-lookup"><span data-stu-id="110b9-125">4</span></span>|<span data-ttu-id="110b9-126">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="110b9-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="110b9-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="110b9-127">atLeastAlphabetic</span></span>|<span data-ttu-id="110b9-128">5 </span><span class="sxs-lookup"><span data-stu-id="110b9-128">5</span></span>|<span data-ttu-id="110b9-129">至少需要字母密码。</span><span class="sxs-lookup"><span data-stu-id="110b9-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="110b9-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="110b9-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="110b9-131">6 </span><span class="sxs-lookup"><span data-stu-id="110b9-131">6</span></span>|<span data-ttu-id="110b9-132">至少需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="110b9-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="110b9-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="110b9-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="110b9-134">7 </span><span class="sxs-lookup"><span data-stu-id="110b9-134">7</span></span>|<span data-ttu-id="110b9-135">至少需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="110b9-135">At least alphanumeric with symbols password required.</span></span>|




