---
title: androidRequiredPasswordComplexity 枚举类型
description: 可在 Android 上设置的密码复杂性类型。 其中一个：无、低、中、高。 这是一个面向 Android 11 + 的 API。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e1e5de9270126a295e05fad789ebd03e392da05c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023521"
---
# <a name="androidrequiredpasswordcomplexity-enum-type"></a><span data-ttu-id="bedd6-105">androidRequiredPasswordComplexity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bedd6-105">androidRequiredPasswordComplexity enum type</span></span>

<span data-ttu-id="bedd6-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bedd6-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bedd6-107">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bedd6-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bedd6-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bedd6-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bedd6-109">可在 Android 上设置的密码复杂性类型。</span><span class="sxs-lookup"><span data-stu-id="bedd6-109">The password complexity types that can be set on Android.</span></span> <span data-ttu-id="bedd6-110">其中一个：无、低、中、高。</span><span class="sxs-lookup"><span data-stu-id="bedd6-110">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="bedd6-111">这是一个面向 Android 11 + 的 API。</span><span class="sxs-lookup"><span data-stu-id="bedd6-111">This is an API targeted to Android 11+.</span></span>

## <a name="members"></a><span data-ttu-id="bedd6-112">成员</span><span class="sxs-lookup"><span data-stu-id="bedd6-112">Members</span></span>
|<span data-ttu-id="bedd6-113">成员</span><span class="sxs-lookup"><span data-stu-id="bedd6-113">Member</span></span>|<span data-ttu-id="bedd6-114">值</span><span class="sxs-lookup"><span data-stu-id="bedd6-114">Value</span></span>|<span data-ttu-id="bedd6-115">说明</span><span class="sxs-lookup"><span data-stu-id="bedd6-115">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bedd6-116">无</span><span class="sxs-lookup"><span data-stu-id="bedd6-116">none</span></span>|<span data-ttu-id="bedd6-117">0</span><span class="sxs-lookup"><span data-stu-id="bedd6-117">0</span></span>|<span data-ttu-id="bedd6-118">设备默认值，无密码。</span><span class="sxs-lookup"><span data-stu-id="bedd6-118">Device default value, no password.</span></span>|
|<span data-ttu-id="bedd6-119">降低</span><span class="sxs-lookup"><span data-stu-id="bedd6-119">low</span></span>|<span data-ttu-id="bedd6-120">1 </span><span class="sxs-lookup"><span data-stu-id="bedd6-120">1</span></span>|<span data-ttu-id="bedd6-121">设备上所需的密码复杂性的类型为 "Android 文档" 定义的 "低"。</span><span class="sxs-lookup"><span data-stu-id="bedd6-121">The required password complexity on the device is of type low as defined by the Android documentation.</span></span>|
|<span data-ttu-id="bedd6-122">中等</span><span class="sxs-lookup"><span data-stu-id="bedd6-122">medium</span></span>|<span data-ttu-id="bedd6-123">2 </span><span class="sxs-lookup"><span data-stu-id="bedd6-123">2</span></span>|<span data-ttu-id="bedd6-124">设备上所需的密码复杂性是由 Android 文档定义的类型中型。</span><span class="sxs-lookup"><span data-stu-id="bedd6-124">The required password complexity on the device is of type medium as defined by the Android documentation.</span></span>|
|<span data-ttu-id="bedd6-125">高效</span><span class="sxs-lookup"><span data-stu-id="bedd6-125">high</span></span>|<span data-ttu-id="bedd6-126">第三章</span><span class="sxs-lookup"><span data-stu-id="bedd6-126">3</span></span>|<span data-ttu-id="bedd6-127">设备上所需的密码复杂性是由 Android 文档定义的 "高" 类型。</span><span class="sxs-lookup"><span data-stu-id="bedd6-127">The required password complexity on the device is of type high as defined by the Android documentation.</span></span>|






