---
title: endpointSecurityConfigurationType 枚举类型
description: 终结点安全策略类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b8eabd459e8816b38d1e908d0da9c0723dca5a16
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48718467"
---
# <a name="endpointsecurityconfigurationtype-enum-type"></a><span data-ttu-id="fe0f5-103">endpointSecurityConfigurationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fe0f5-103">endpointSecurityConfigurationType enum type</span></span>

<span data-ttu-id="fe0f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe0f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe0f5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fe0f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe0f5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe0f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe0f5-107">终结点安全策略类型。</span><span class="sxs-lookup"><span data-stu-id="fe0f5-107">The endpoint security policy type.</span></span>

## <a name="members"></a><span data-ttu-id="fe0f5-108">成员</span><span class="sxs-lookup"><span data-stu-id="fe0f5-108">Members</span></span>
|<span data-ttu-id="fe0f5-109">成员</span><span class="sxs-lookup"><span data-stu-id="fe0f5-109">Member</span></span>|<span data-ttu-id="fe0f5-110">值</span><span class="sxs-lookup"><span data-stu-id="fe0f5-110">Value</span></span>|<span data-ttu-id="fe0f5-111">说明</span><span class="sxs-lookup"><span data-stu-id="fe0f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe0f5-112">unknown</span><span class="sxs-lookup"><span data-stu-id="fe0f5-112">unknown</span></span>|<span data-ttu-id="fe0f5-113">0</span><span class="sxs-lookup"><span data-stu-id="fe0f5-113">0</span></span>|<span data-ttu-id="fe0f5-114">陌生.</span><span class="sxs-lookup"><span data-stu-id="fe0f5-114">Unknown.</span></span>|
|<span data-ttu-id="fe0f5-115">程序</span><span class="sxs-lookup"><span data-stu-id="fe0f5-115">antivirus</span></span>|<span data-ttu-id="fe0f5-116">1</span><span class="sxs-lookup"><span data-stu-id="fe0f5-116">1</span></span>|<span data-ttu-id="fe0f5-117">程序.</span><span class="sxs-lookup"><span data-stu-id="fe0f5-117">Antivirus.</span></span>|
|<span data-ttu-id="fe0f5-118">diskEncryption</span><span class="sxs-lookup"><span data-stu-id="fe0f5-118">diskEncryption</span></span>|<span data-ttu-id="fe0f5-119">双面</span><span class="sxs-lookup"><span data-stu-id="fe0f5-119">2</span></span>|<span data-ttu-id="fe0f5-120">磁盘加密。</span><span class="sxs-lookup"><span data-stu-id="fe0f5-120">Disk encryption.</span></span>|
|<span data-ttu-id="fe0f5-121">firewall</span><span class="sxs-lookup"><span data-stu-id="fe0f5-121">firewall</span></span>|<span data-ttu-id="fe0f5-122">第三章</span><span class="sxs-lookup"><span data-stu-id="fe0f5-122">3</span></span>|<span data-ttu-id="fe0f5-123">Firewall.</span><span class="sxs-lookup"><span data-stu-id="fe0f5-123">Firewall.</span></span>|
|<span data-ttu-id="fe0f5-124">endpointDetectionAndResponse</span><span class="sxs-lookup"><span data-stu-id="fe0f5-124">endpointDetectionAndResponse</span></span>|<span data-ttu-id="fe0f5-125">4 </span><span class="sxs-lookup"><span data-stu-id="fe0f5-125">4</span></span>|<span data-ttu-id="fe0f5-126">终结点检测和响应。</span><span class="sxs-lookup"><span data-stu-id="fe0f5-126">Endpoint detection and response.</span></span>|
|<span data-ttu-id="fe0f5-127">attackSurfaceReduction</span><span class="sxs-lookup"><span data-stu-id="fe0f5-127">attackSurfaceReduction</span></span>|<span data-ttu-id="fe0f5-128">5 </span><span class="sxs-lookup"><span data-stu-id="fe0f5-128">5</span></span>|<span data-ttu-id="fe0f5-129">攻击面减少。</span><span class="sxs-lookup"><span data-stu-id="fe0f5-129">Attack surface reduction.</span></span>|
|<span data-ttu-id="fe0f5-130">accountProtection</span><span class="sxs-lookup"><span data-stu-id="fe0f5-130">accountProtection</span></span>|<span data-ttu-id="fe0f5-131">6 </span><span class="sxs-lookup"><span data-stu-id="fe0f5-131">6</span></span>|<span data-ttu-id="fe0f5-132">帐户保护。</span><span class="sxs-lookup"><span data-stu-id="fe0f5-132">Account protection.</span></span>|





