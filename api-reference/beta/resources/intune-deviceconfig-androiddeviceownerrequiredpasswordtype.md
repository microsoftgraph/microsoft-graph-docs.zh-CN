---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略需要密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79d71fbabc4597c87c9cee782904334e2f12d7e8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172588"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="f4954-103">androidDeviceOwnerRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f4954-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="f4954-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4954-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4954-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4954-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4954-106">Android 设备所有者策略需要密码类型。</span><span class="sxs-lookup"><span data-stu-id="f4954-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="f4954-107">成员</span><span class="sxs-lookup"><span data-stu-id="f4954-107">Members</span></span>
|<span data-ttu-id="f4954-108">成员</span><span class="sxs-lookup"><span data-stu-id="f4954-108">Member</span></span>|<span data-ttu-id="f4954-109">值</span><span class="sxs-lookup"><span data-stu-id="f4954-109">Value</span></span>|<span data-ttu-id="f4954-110">说明</span><span class="sxs-lookup"><span data-stu-id="f4954-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4954-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f4954-111">deviceDefault</span></span>|<span data-ttu-id="f4954-112">0</span><span class="sxs-lookup"><span data-stu-id="f4954-112">0</span></span>|<span data-ttu-id="f4954-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="f4954-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="f4954-114">必需</span><span class="sxs-lookup"><span data-stu-id="f4954-114">required</span></span>|<span data-ttu-id="f4954-115">1</span><span class="sxs-lookup"><span data-stu-id="f4954-115">1</span></span>|<span data-ttu-id="f4954-116">必须设置密码, 但类型没有限制。</span><span class="sxs-lookup"><span data-stu-id="f4954-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="f4954-117">位数</span><span class="sxs-lookup"><span data-stu-id="f4954-117">numeric</span></span>|<span data-ttu-id="f4954-118">双面</span><span class="sxs-lookup"><span data-stu-id="f4954-118">2</span></span>|<span data-ttu-id="f4954-119">至少为数值。</span><span class="sxs-lookup"><span data-stu-id="f4954-119">At least numeric.</span></span>|
|<span data-ttu-id="f4954-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="f4954-120">numericComplex</span></span>|<span data-ttu-id="f4954-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f4954-121">3</span></span>|<span data-ttu-id="f4954-122">至少不带重复或有序序列的数字。</span><span class="sxs-lookup"><span data-stu-id="f4954-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="f4954-123">字母</span><span class="sxs-lookup"><span data-stu-id="f4954-123">alphabetic</span></span>|<span data-ttu-id="f4954-124">4</span><span class="sxs-lookup"><span data-stu-id="f4954-124">4</span></span>|<span data-ttu-id="f4954-125">至少为字母密码。</span><span class="sxs-lookup"><span data-stu-id="f4954-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="f4954-126">字母数字</span><span class="sxs-lookup"><span data-stu-id="f4954-126">alphanumeric</span></span>|<span data-ttu-id="f4954-127">5</span><span class="sxs-lookup"><span data-stu-id="f4954-127">5</span></span>|<span data-ttu-id="f4954-128">至少为字母数字密码</span><span class="sxs-lookup"><span data-stu-id="f4954-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="f4954-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="f4954-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="f4954-130">型</span><span class="sxs-lookup"><span data-stu-id="f4954-130">6</span></span>|<span data-ttu-id="f4954-131">至少带有符号的字母数字。</span><span class="sxs-lookup"><span data-stu-id="f4954-131">At least alphanumeric with symbols.</span></span>|




