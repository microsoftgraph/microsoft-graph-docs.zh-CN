---
title: endpointSecurityConfigurationType 枚举类型
description: 终结点安全策略类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6f46b07f62591b33f34b8e847b406763a0047f15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993635"
---
# <a name="endpointsecurityconfigurationtype-enum-type"></a><span data-ttu-id="2dd1e-103">endpointSecurityConfigurationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2dd1e-103">endpointSecurityConfigurationType enum type</span></span>

<span data-ttu-id="2dd1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dd1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2dd1e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2dd1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dd1e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2dd1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dd1e-107">终结点安全策略类型。</span><span class="sxs-lookup"><span data-stu-id="2dd1e-107">The endpoint security policy type.</span></span>

## <a name="members"></a><span data-ttu-id="2dd1e-108">成员</span><span class="sxs-lookup"><span data-stu-id="2dd1e-108">Members</span></span>
|<span data-ttu-id="2dd1e-109">成员</span><span class="sxs-lookup"><span data-stu-id="2dd1e-109">Member</span></span>|<span data-ttu-id="2dd1e-110">值</span><span class="sxs-lookup"><span data-stu-id="2dd1e-110">Value</span></span>|<span data-ttu-id="2dd1e-111">说明</span><span class="sxs-lookup"><span data-stu-id="2dd1e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dd1e-112">unknown</span><span class="sxs-lookup"><span data-stu-id="2dd1e-112">unknown</span></span>|<span data-ttu-id="2dd1e-113">0</span><span class="sxs-lookup"><span data-stu-id="2dd1e-113">0</span></span>|<span data-ttu-id="2dd1e-114">陌生.</span><span class="sxs-lookup"><span data-stu-id="2dd1e-114">Unknown.</span></span>|
|<span data-ttu-id="2dd1e-115">程序</span><span class="sxs-lookup"><span data-stu-id="2dd1e-115">antivirus</span></span>|<span data-ttu-id="2dd1e-116">1 </span><span class="sxs-lookup"><span data-stu-id="2dd1e-116">1</span></span>|<span data-ttu-id="2dd1e-117">程序.</span><span class="sxs-lookup"><span data-stu-id="2dd1e-117">Antivirus.</span></span>|
|<span data-ttu-id="2dd1e-118">diskEncryption</span><span class="sxs-lookup"><span data-stu-id="2dd1e-118">diskEncryption</span></span>|<span data-ttu-id="2dd1e-119">2 </span><span class="sxs-lookup"><span data-stu-id="2dd1e-119">2</span></span>|<span data-ttu-id="2dd1e-120">磁盘加密。</span><span class="sxs-lookup"><span data-stu-id="2dd1e-120">Disk encryption.</span></span>|
|<span data-ttu-id="2dd1e-121">firewall</span><span class="sxs-lookup"><span data-stu-id="2dd1e-121">firewall</span></span>|<span data-ttu-id="2dd1e-122">第三章</span><span class="sxs-lookup"><span data-stu-id="2dd1e-122">3</span></span>|<span data-ttu-id="2dd1e-123">Firewall.</span><span class="sxs-lookup"><span data-stu-id="2dd1e-123">Firewall.</span></span>|
|<span data-ttu-id="2dd1e-124">endpointDetectionAndResponse</span><span class="sxs-lookup"><span data-stu-id="2dd1e-124">endpointDetectionAndResponse</span></span>|<span data-ttu-id="2dd1e-125">4 </span><span class="sxs-lookup"><span data-stu-id="2dd1e-125">4</span></span>|<span data-ttu-id="2dd1e-126">终结点检测和响应。</span><span class="sxs-lookup"><span data-stu-id="2dd1e-126">Endpoint detection and response.</span></span>|
|<span data-ttu-id="2dd1e-127">attackSurfaceReduction</span><span class="sxs-lookup"><span data-stu-id="2dd1e-127">attackSurfaceReduction</span></span>|<span data-ttu-id="2dd1e-128">5 </span><span class="sxs-lookup"><span data-stu-id="2dd1e-128">5</span></span>|<span data-ttu-id="2dd1e-129">攻击面减少。</span><span class="sxs-lookup"><span data-stu-id="2dd1e-129">Attack surface reduction.</span></span>|
|<span data-ttu-id="2dd1e-130">accountProtection</span><span class="sxs-lookup"><span data-stu-id="2dd1e-130">accountProtection</span></span>|<span data-ttu-id="2dd1e-131">6 </span><span class="sxs-lookup"><span data-stu-id="2dd1e-131">6</span></span>|<span data-ttu-id="2dd1e-132">帐户保护。</span><span class="sxs-lookup"><span data-stu-id="2dd1e-132">Account protection.</span></span>|






