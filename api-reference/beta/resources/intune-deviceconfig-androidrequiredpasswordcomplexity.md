---
title: androidRequiredPasswordComplexity 枚举类型
description: 可在 Android 上设置的密码复杂性类型。 其中一个：无、低、中、高。 这是一个面向 Android 11 + 的 API。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 18ca4c424a97444009a85f3499f6d50bc3fa294a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231687"
---
# <a name="androidrequiredpasswordcomplexity-enum-type"></a><span data-ttu-id="4e0e0-105">androidRequiredPasswordComplexity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4e0e0-105">androidRequiredPasswordComplexity enum type</span></span>

<span data-ttu-id="4e0e0-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e0e0-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e0e0-107">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e0e0-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e0e0-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e0e0-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e0e0-109">可在 Android 上设置的密码复杂性类型。</span><span class="sxs-lookup"><span data-stu-id="4e0e0-109">The password complexity types that can be set on Android.</span></span> <span data-ttu-id="4e0e0-110">其中一个：无、低、中、高。</span><span class="sxs-lookup"><span data-stu-id="4e0e0-110">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="4e0e0-111">这是一个面向 Android 11 + 的 API。</span><span class="sxs-lookup"><span data-stu-id="4e0e0-111">This is an API targeted to Android 11+.</span></span>

## <a name="members"></a><span data-ttu-id="4e0e0-112">成员</span><span class="sxs-lookup"><span data-stu-id="4e0e0-112">Members</span></span>
|<span data-ttu-id="4e0e0-113">成员</span><span class="sxs-lookup"><span data-stu-id="4e0e0-113">Member</span></span>|<span data-ttu-id="4e0e0-114">值</span><span class="sxs-lookup"><span data-stu-id="4e0e0-114">Value</span></span>|<span data-ttu-id="4e0e0-115">说明</span><span class="sxs-lookup"><span data-stu-id="4e0e0-115">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e0e0-116">无</span><span class="sxs-lookup"><span data-stu-id="4e0e0-116">none</span></span>|<span data-ttu-id="4e0e0-117">0</span><span class="sxs-lookup"><span data-stu-id="4e0e0-117">0</span></span>|<span data-ttu-id="4e0e0-118">设备默认值，无密码。</span><span class="sxs-lookup"><span data-stu-id="4e0e0-118">Device default value, no password.</span></span>|
|<span data-ttu-id="4e0e0-119">降低</span><span class="sxs-lookup"><span data-stu-id="4e0e0-119">low</span></span>|<span data-ttu-id="4e0e0-120">1</span><span class="sxs-lookup"><span data-stu-id="4e0e0-120">1</span></span>|<span data-ttu-id="4e0e0-121">设备上所需的密码复杂性的类型为 "Android 文档" 定义的 "低"。</span><span class="sxs-lookup"><span data-stu-id="4e0e0-121">The required password complexity on the device is of type low as defined by the Android documentation.</span></span>|
|<span data-ttu-id="4e0e0-122">中等</span><span class="sxs-lookup"><span data-stu-id="4e0e0-122">medium</span></span>|<span data-ttu-id="4e0e0-123">双面</span><span class="sxs-lookup"><span data-stu-id="4e0e0-123">2</span></span>|<span data-ttu-id="4e0e0-124">设备上所需的密码复杂性是由 Android 文档定义的类型中型。</span><span class="sxs-lookup"><span data-stu-id="4e0e0-124">The required password complexity on the device is of type medium as defined by the Android documentation.</span></span>|
|<span data-ttu-id="4e0e0-125">高效</span><span class="sxs-lookup"><span data-stu-id="4e0e0-125">high</span></span>|<span data-ttu-id="4e0e0-126">第三章</span><span class="sxs-lookup"><span data-stu-id="4e0e0-126">3</span></span>|<span data-ttu-id="4e0e0-127">设备上所需的密码复杂性是由 Android 文档定义的 "高" 类型。</span><span class="sxs-lookup"><span data-stu-id="4e0e0-127">The required password complexity on the device is of type high as defined by the Android documentation.</span></span>|




