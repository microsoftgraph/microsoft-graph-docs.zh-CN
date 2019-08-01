---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9154a78af87dbef125e5d211aba284d7a0023e84
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027647"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="0ea1c-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0ea1c-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="0ea1c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ea1c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ea1c-105">对等分发的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="0ea1c-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="0ea1c-106">成员</span><span class="sxs-lookup"><span data-stu-id="0ea1c-106">Members</span></span>
|<span data-ttu-id="0ea1c-107">成员</span><span class="sxs-lookup"><span data-stu-id="0ea1c-107">Member</span></span>|<span data-ttu-id="0ea1c-108">值</span><span class="sxs-lookup"><span data-stu-id="0ea1c-108">Value</span></span>|<span data-ttu-id="0ea1c-109">说明</span><span class="sxs-lookup"><span data-stu-id="0ea1c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ea1c-110">定制</span><span class="sxs-lookup"><span data-stu-id="0ea1c-110">userDefined</span></span>|<span data-ttu-id="0ea1c-111">0</span><span class="sxs-lookup"><span data-stu-id="0ea1c-111">0</span></span>|<span data-ttu-id="0ea1c-112">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="0ea1c-112">Allow the user to set.</span></span>|
|<span data-ttu-id="0ea1c-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="0ea1c-113">httpOnly</span></span>|<span data-ttu-id="0ea1c-114">1</span><span class="sxs-lookup"><span data-stu-id="0ea1c-114">1</span></span>|<span data-ttu-id="0ea1c-115">仅限 HTTP, 无对等</span><span class="sxs-lookup"><span data-stu-id="0ea1c-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="0ea1c-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="0ea1c-116">httpWithPeeringNat</span></span>|<span data-ttu-id="0ea1c-117">双面</span><span class="sxs-lookup"><span data-stu-id="0ea1c-117">2</span></span>|<span data-ttu-id="0ea1c-118">OS 默认值–在同一网络地址转换器后具有对等的 Http 混合</span><span class="sxs-lookup"><span data-stu-id="0ea1c-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="0ea1c-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="0ea1c-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="0ea1c-120">第三章</span><span class="sxs-lookup"><span data-stu-id="0ea1c-120">3</span></span>|<span data-ttu-id="0ea1c-121">通过专用组与对等互连的 HTTP 混合</span><span class="sxs-lookup"><span data-stu-id="0ea1c-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="0ea1c-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="0ea1c-122">httpWithInternetPeering</span></span>|<span data-ttu-id="0ea1c-123">4</span><span class="sxs-lookup"><span data-stu-id="0ea1c-123">4</span></span>|<span data-ttu-id="0ea1c-124">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="0ea1c-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="0ea1c-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="0ea1c-125">simpleDownload</span></span>|<span data-ttu-id="0ea1c-126">99</span><span class="sxs-lookup"><span data-stu-id="0ea1c-126">99</span></span>|<span data-ttu-id="0ea1c-127">无对等的简单下载模式</span><span class="sxs-lookup"><span data-stu-id="0ea1c-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="0ea1c-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="0ea1c-128">bypassMode</span></span>|<span data-ttu-id="0ea1c-129">100</span><span class="sxs-lookup"><span data-stu-id="0ea1c-129">100</span></span>|<span data-ttu-id="0ea1c-130">旁路模式。</span><span class="sxs-lookup"><span data-stu-id="0ea1c-130">Bypass mode.</span></span> <span data-ttu-id="0ea1c-131">请勿使用传递优化和改用 BITS</span><span class="sxs-lookup"><span data-stu-id="0ea1c-131">Do not use Delivery Optimization and use BITS instead</span></span>|



