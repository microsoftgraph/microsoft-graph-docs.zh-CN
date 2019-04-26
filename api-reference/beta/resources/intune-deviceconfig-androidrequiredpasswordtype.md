---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d70ac87a0e8e3e8d97705b46f5d6ec63d85fbcac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562494"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="f1cc8-103">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f1cc8-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="f1cc8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1cc8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1cc8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1cc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1cc8-106">Android 必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="f1cc8-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="f1cc8-107">成员</span><span class="sxs-lookup"><span data-stu-id="f1cc8-107">Members</span></span>
|<span data-ttu-id="f1cc8-108">成员</span><span class="sxs-lookup"><span data-stu-id="f1cc8-108">Member</span></span>|<span data-ttu-id="f1cc8-109">值</span><span class="sxs-lookup"><span data-stu-id="f1cc8-109">Value</span></span>|<span data-ttu-id="f1cc8-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1cc8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1cc8-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f1cc8-111">deviceDefault</span></span>|<span data-ttu-id="f1cc8-112">0</span><span class="sxs-lookup"><span data-stu-id="f1cc8-112">0</span></span>|<span data-ttu-id="f1cc8-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="f1cc8-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="f1cc8-114">字母</span><span class="sxs-lookup"><span data-stu-id="f1cc8-114">alphabetic</span></span>|<span data-ttu-id="f1cc8-115">1</span><span class="sxs-lookup"><span data-stu-id="f1cc8-115">1</span></span>|<span data-ttu-id="f1cc8-116">要求字母密码。</span><span class="sxs-lookup"><span data-stu-id="f1cc8-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="f1cc8-117">字母数字</span><span class="sxs-lookup"><span data-stu-id="f1cc8-117">alphanumeric</span></span>|<span data-ttu-id="f1cc8-118">2 </span><span class="sxs-lookup"><span data-stu-id="f1cc8-118">2</span></span>|<span data-ttu-id="f1cc8-119">需要字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="f1cc8-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="f1cc8-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="f1cc8-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="f1cc8-121">3 </span><span class="sxs-lookup"><span data-stu-id="f1cc8-121">3</span></span>|<span data-ttu-id="f1cc8-122">需要带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="f1cc8-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="f1cc8-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="f1cc8-123">lowSecurityBiometric</span></span>|<span data-ttu-id="f1cc8-124">4 </span><span class="sxs-lookup"><span data-stu-id="f1cc8-124">4</span></span>|<span data-ttu-id="f1cc8-125">要求低安全基于生物特征的密码。</span><span class="sxs-lookup"><span data-stu-id="f1cc8-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="f1cc8-126">位数</span><span class="sxs-lookup"><span data-stu-id="f1cc8-126">numeric</span></span>|<span data-ttu-id="f1cc8-127">5 </span><span class="sxs-lookup"><span data-stu-id="f1cc8-127">5</span></span>|<span data-ttu-id="f1cc8-128">需要数字密码。</span><span class="sxs-lookup"><span data-stu-id="f1cc8-128">Numeric password required.</span></span>|
|<span data-ttu-id="f1cc8-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="f1cc8-129">numericComplex</span></span>|<span data-ttu-id="f1cc8-130">6 </span><span class="sxs-lookup"><span data-stu-id="f1cc8-130">6</span></span>|<span data-ttu-id="f1cc8-131">需要数字复杂密码。</span><span class="sxs-lookup"><span data-stu-id="f1cc8-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="f1cc8-132">任意</span><span class="sxs-lookup"><span data-stu-id="f1cc8-132">any</span></span>|<span data-ttu-id="f1cc8-133">7 </span><span class="sxs-lookup"><span data-stu-id="f1cc8-133">7</span></span>|<span data-ttu-id="f1cc8-134">需要密码或模式, 可以接受。</span><span class="sxs-lookup"><span data-stu-id="f1cc8-134">A password or pattern is required, and any is acceptable.</span></span>|





