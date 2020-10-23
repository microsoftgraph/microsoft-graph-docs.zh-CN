---
title: androidRequiredPasswordComplexity 枚举类型
description: 可在 Android 上设置的密码复杂性类型。 其中一个：无、低、中、高。 这是一个面向 Android 11 + 的 API。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f26f1e55e4f4703a06db6a7b2d44fb1b3cfd753a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724619"
---
# <a name="androidrequiredpasswordcomplexity-enum-type"></a><span data-ttu-id="3e53b-105">androidRequiredPasswordComplexity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3e53b-105">androidRequiredPasswordComplexity enum type</span></span>

<span data-ttu-id="3e53b-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e53b-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e53b-107">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e53b-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e53b-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e53b-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e53b-109">可在 Android 上设置的密码复杂性类型。</span><span class="sxs-lookup"><span data-stu-id="3e53b-109">The password complexity types that can be set on Android.</span></span> <span data-ttu-id="3e53b-110">其中一个：无、低、中、高。</span><span class="sxs-lookup"><span data-stu-id="3e53b-110">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="3e53b-111">这是一个面向 Android 11 + 的 API。</span><span class="sxs-lookup"><span data-stu-id="3e53b-111">This is an API targeted to Android 11+.</span></span>

## <a name="members"></a><span data-ttu-id="3e53b-112">成员</span><span class="sxs-lookup"><span data-stu-id="3e53b-112">Members</span></span>
|<span data-ttu-id="3e53b-113">成员</span><span class="sxs-lookup"><span data-stu-id="3e53b-113">Member</span></span>|<span data-ttu-id="3e53b-114">值</span><span class="sxs-lookup"><span data-stu-id="3e53b-114">Value</span></span>|<span data-ttu-id="3e53b-115">说明</span><span class="sxs-lookup"><span data-stu-id="3e53b-115">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e53b-116">无</span><span class="sxs-lookup"><span data-stu-id="3e53b-116">none</span></span>|<span data-ttu-id="3e53b-117">0</span><span class="sxs-lookup"><span data-stu-id="3e53b-117">0</span></span>|<span data-ttu-id="3e53b-118">设备默认值，无密码。</span><span class="sxs-lookup"><span data-stu-id="3e53b-118">Device default value, no password.</span></span>|
|<span data-ttu-id="3e53b-119">降低</span><span class="sxs-lookup"><span data-stu-id="3e53b-119">low</span></span>|<span data-ttu-id="3e53b-120">1</span><span class="sxs-lookup"><span data-stu-id="3e53b-120">1</span></span>|<span data-ttu-id="3e53b-121">设备上所需的密码复杂性的类型为 "Android 文档" 定义的 "低"。</span><span class="sxs-lookup"><span data-stu-id="3e53b-121">The required password complexity on the device is of type low as defined by the Android documentation.</span></span>|
|<span data-ttu-id="3e53b-122">中等</span><span class="sxs-lookup"><span data-stu-id="3e53b-122">medium</span></span>|<span data-ttu-id="3e53b-123">双面</span><span class="sxs-lookup"><span data-stu-id="3e53b-123">2</span></span>|<span data-ttu-id="3e53b-124">设备上所需的密码复杂性是由 Android 文档定义的类型中型。</span><span class="sxs-lookup"><span data-stu-id="3e53b-124">The required password complexity on the device is of type medium as defined by the Android documentation.</span></span>|
|<span data-ttu-id="3e53b-125">高效</span><span class="sxs-lookup"><span data-stu-id="3e53b-125">high</span></span>|<span data-ttu-id="3e53b-126">第三章</span><span class="sxs-lookup"><span data-stu-id="3e53b-126">3</span></span>|<span data-ttu-id="3e53b-127">设备上所需的密码复杂性是由 Android 文档定义的 "高" 类型。</span><span class="sxs-lookup"><span data-stu-id="3e53b-127">The required password complexity on the device is of type high as defined by the Android documentation.</span></span>|





