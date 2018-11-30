---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略要求密码类型。
ms.openlocfilehash: 16f4bc59f2b4fa9f37989d1bc1978cdfacb2892c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045885"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="d75a7-103">androidDeviceOwnerRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d75a7-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="d75a7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d75a7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d75a7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d75a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d75a7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d75a7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d75a7-107">Android 设备所有者策略要求密码类型。</span><span class="sxs-lookup"><span data-stu-id="d75a7-107">Android Device Owner policy required password type.</span></span>
## <a name="members"></a><span data-ttu-id="d75a7-108">成员</span><span class="sxs-lookup"><span data-stu-id="d75a7-108">Members</span></span>
|<span data-ttu-id="d75a7-109">成员</span><span class="sxs-lookup"><span data-stu-id="d75a7-109">Member</span></span>|<span data-ttu-id="d75a7-110">值</span><span class="sxs-lookup"><span data-stu-id="d75a7-110">Value</span></span>|<span data-ttu-id="d75a7-111">说明</span><span class="sxs-lookup"><span data-stu-id="d75a7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d75a7-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d75a7-112">deviceDefault</span></span>|<span data-ttu-id="d75a7-113">0</span><span class="sxs-lookup"><span data-stu-id="d75a7-113">0</span></span>|<span data-ttu-id="d75a7-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="d75a7-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="d75a7-115">必需</span><span class="sxs-lookup"><span data-stu-id="d75a7-115">required</span></span>|<span data-ttu-id="d75a7-116">1</span><span class="sxs-lookup"><span data-stu-id="d75a7-116">1</span></span>|<span data-ttu-id="d75a7-117">必须有一密码，但没有任何限制类型。</span><span class="sxs-lookup"><span data-stu-id="d75a7-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="d75a7-118">数值</span><span class="sxs-lookup"><span data-stu-id="d75a7-118">numeric</span></span>|<span data-ttu-id="d75a7-119">2</span><span class="sxs-lookup"><span data-stu-id="d75a7-119">2</span></span>|<span data-ttu-id="d75a7-120">在至少数值。</span><span class="sxs-lookup"><span data-stu-id="d75a7-120">At least numeric.</span></span>|
|<span data-ttu-id="d75a7-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="d75a7-121">numericComplex</span></span>|<span data-ttu-id="d75a7-122">3</span><span class="sxs-lookup"><span data-stu-id="d75a7-122">3</span></span>|<span data-ttu-id="d75a7-123">在与没有重复或有序序列至少数值。</span><span class="sxs-lookup"><span data-stu-id="d75a7-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="d75a7-124">字母</span><span class="sxs-lookup"><span data-stu-id="d75a7-124">alphabetic</span></span>|<span data-ttu-id="d75a7-125">4</span><span class="sxs-lookup"><span data-stu-id="d75a7-125">4</span></span>|<span data-ttu-id="d75a7-126">至少字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="d75a7-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="d75a7-127">字母数字</span><span class="sxs-lookup"><span data-stu-id="d75a7-127">alphanumeric</span></span>|<span data-ttu-id="d75a7-128">5</span><span class="sxs-lookup"><span data-stu-id="d75a7-128">5</span></span>|<span data-ttu-id="d75a7-129">至少字母数字密码</span><span class="sxs-lookup"><span data-stu-id="d75a7-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="d75a7-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="d75a7-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="d75a7-131">6</span><span class="sxs-lookup"><span data-stu-id="d75a7-131">6</span></span>|<span data-ttu-id="d75a7-132">替换为长划线至少字母数字。</span><span class="sxs-lookup"><span data-stu-id="d75a7-132">At least alphanumeric with symbols.</span></span>|





