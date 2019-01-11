---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略要求密码类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c53cc67d01886b76a20eef149a59c1d1fef4fc83
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887645"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="97a88-103">androidDeviceOwnerRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="97a88-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="97a88-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="97a88-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97a88-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="97a88-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97a88-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="97a88-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97a88-107">Android 设备所有者策略要求密码类型。</span><span class="sxs-lookup"><span data-stu-id="97a88-107">Android Device Owner policy required password type.</span></span>
## <a name="members"></a><span data-ttu-id="97a88-108">成员</span><span class="sxs-lookup"><span data-stu-id="97a88-108">Members</span></span>
|<span data-ttu-id="97a88-109">成员</span><span class="sxs-lookup"><span data-stu-id="97a88-109">Member</span></span>|<span data-ttu-id="97a88-110">值</span><span class="sxs-lookup"><span data-stu-id="97a88-110">Value</span></span>|<span data-ttu-id="97a88-111">Description</span><span class="sxs-lookup"><span data-stu-id="97a88-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97a88-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="97a88-112">deviceDefault</span></span>|<span data-ttu-id="97a88-113">0</span><span class="sxs-lookup"><span data-stu-id="97a88-113">0</span></span>|<span data-ttu-id="97a88-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="97a88-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="97a88-115">必需</span><span class="sxs-lookup"><span data-stu-id="97a88-115">required</span></span>|<span data-ttu-id="97a88-116">1</span><span class="sxs-lookup"><span data-stu-id="97a88-116">1</span></span>|<span data-ttu-id="97a88-117">必须有一密码，但没有任何限制类型。</span><span class="sxs-lookup"><span data-stu-id="97a88-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="97a88-118">数值</span><span class="sxs-lookup"><span data-stu-id="97a88-118">numeric</span></span>|<span data-ttu-id="97a88-119">2</span><span class="sxs-lookup"><span data-stu-id="97a88-119">2</span></span>|<span data-ttu-id="97a88-120">在至少数值。</span><span class="sxs-lookup"><span data-stu-id="97a88-120">At least numeric.</span></span>|
|<span data-ttu-id="97a88-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="97a88-121">numericComplex</span></span>|<span data-ttu-id="97a88-122">3</span><span class="sxs-lookup"><span data-stu-id="97a88-122">3</span></span>|<span data-ttu-id="97a88-123">在与没有重复或有序序列至少数值。</span><span class="sxs-lookup"><span data-stu-id="97a88-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="97a88-124">字母</span><span class="sxs-lookup"><span data-stu-id="97a88-124">alphabetic</span></span>|<span data-ttu-id="97a88-125">4</span><span class="sxs-lookup"><span data-stu-id="97a88-125">4</span></span>|<span data-ttu-id="97a88-126">至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="97a88-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="97a88-127">字母数字</span><span class="sxs-lookup"><span data-stu-id="97a88-127">alphanumeric</span></span>|<span data-ttu-id="97a88-128">5</span><span class="sxs-lookup"><span data-stu-id="97a88-128">5</span></span>|<span data-ttu-id="97a88-129">至少字母数字密码</span><span class="sxs-lookup"><span data-stu-id="97a88-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="97a88-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="97a88-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="97a88-131">6</span><span class="sxs-lookup"><span data-stu-id="97a88-131">6</span></span>|<span data-ttu-id="97a88-132">替换为长划线至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="97a88-132">At least alphanumeric with symbols.</span></span>|





