---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略要求密码类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c405cf3a69597994d5539427698baa92cabd3904
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403537"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="146d9-103">androidDeviceOwnerRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="146d9-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="146d9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="146d9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="146d9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="146d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="146d9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="146d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="146d9-107">Android 设备所有者策略要求密码类型。</span><span class="sxs-lookup"><span data-stu-id="146d9-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="146d9-108">成员</span><span class="sxs-lookup"><span data-stu-id="146d9-108">Members</span></span>
|<span data-ttu-id="146d9-109">成员</span><span class="sxs-lookup"><span data-stu-id="146d9-109">Member</span></span>|<span data-ttu-id="146d9-110">值</span><span class="sxs-lookup"><span data-stu-id="146d9-110">Value</span></span>|<span data-ttu-id="146d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="146d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="146d9-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="146d9-112">deviceDefault</span></span>|<span data-ttu-id="146d9-113">0</span><span class="sxs-lookup"><span data-stu-id="146d9-113">0</span></span>|<span data-ttu-id="146d9-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="146d9-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="146d9-115">必需</span><span class="sxs-lookup"><span data-stu-id="146d9-115">required</span></span>|<span data-ttu-id="146d9-116">1</span><span class="sxs-lookup"><span data-stu-id="146d9-116">1</span></span>|<span data-ttu-id="146d9-117">必须有一密码，但没有任何限制类型。</span><span class="sxs-lookup"><span data-stu-id="146d9-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="146d9-118">数值</span><span class="sxs-lookup"><span data-stu-id="146d9-118">numeric</span></span>|<span data-ttu-id="146d9-119">2</span><span class="sxs-lookup"><span data-stu-id="146d9-119">2</span></span>|<span data-ttu-id="146d9-120">在至少数值。</span><span class="sxs-lookup"><span data-stu-id="146d9-120">At least numeric.</span></span>|
|<span data-ttu-id="146d9-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="146d9-121">numericComplex</span></span>|<span data-ttu-id="146d9-122">3</span><span class="sxs-lookup"><span data-stu-id="146d9-122">3</span></span>|<span data-ttu-id="146d9-123">在与没有重复或有序序列至少数值。</span><span class="sxs-lookup"><span data-stu-id="146d9-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="146d9-124">字母</span><span class="sxs-lookup"><span data-stu-id="146d9-124">alphabetic</span></span>|<span data-ttu-id="146d9-125">4</span><span class="sxs-lookup"><span data-stu-id="146d9-125">4</span></span>|<span data-ttu-id="146d9-126">至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="146d9-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="146d9-127">字母数字</span><span class="sxs-lookup"><span data-stu-id="146d9-127">alphanumeric</span></span>|<span data-ttu-id="146d9-128">5</span><span class="sxs-lookup"><span data-stu-id="146d9-128">5</span></span>|<span data-ttu-id="146d9-129">至少字母数字密码</span><span class="sxs-lookup"><span data-stu-id="146d9-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="146d9-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="146d9-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="146d9-131">6</span><span class="sxs-lookup"><span data-stu-id="146d9-131">6</span></span>|<span data-ttu-id="146d9-132">替换为长划线至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="146d9-132">At least alphanumeric with symbols.</span></span>|




