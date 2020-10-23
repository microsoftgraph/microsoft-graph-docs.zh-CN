---
title: endpointSecurityConfigurationProfileType 枚举类型
description: 终结点安全策略配置文件类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3bf94da084e59faaa5a63e3b2b5a783c12f6f9d2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48718474"
---
# <a name="endpointsecurityconfigurationprofiletype-enum-type"></a><span data-ttu-id="c6f48-103">endpointSecurityConfigurationProfileType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c6f48-103">endpointSecurityConfigurationProfileType enum type</span></span>

<span data-ttu-id="c6f48-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6f48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6f48-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6f48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6f48-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6f48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6f48-107">终结点安全策略配置文件类型。</span><span class="sxs-lookup"><span data-stu-id="c6f48-107">The endpoint security policy profile type.</span></span>

## <a name="members"></a><span data-ttu-id="c6f48-108">成员</span><span class="sxs-lookup"><span data-stu-id="c6f48-108">Members</span></span>
|<span data-ttu-id="c6f48-109">成员</span><span class="sxs-lookup"><span data-stu-id="c6f48-109">Member</span></span>|<span data-ttu-id="c6f48-110">值</span><span class="sxs-lookup"><span data-stu-id="c6f48-110">Value</span></span>|<span data-ttu-id="c6f48-111">说明</span><span class="sxs-lookup"><span data-stu-id="c6f48-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6f48-112">unknown</span><span class="sxs-lookup"><span data-stu-id="c6f48-112">unknown</span></span>|<span data-ttu-id="c6f48-113">0</span><span class="sxs-lookup"><span data-stu-id="c6f48-113">0</span></span>|<span data-ttu-id="c6f48-114">陌生.</span><span class="sxs-lookup"><span data-stu-id="c6f48-114">Unknown.</span></span>|
|<span data-ttu-id="c6f48-115">程序</span><span class="sxs-lookup"><span data-stu-id="c6f48-115">antivirus</span></span>|<span data-ttu-id="c6f48-116">1</span><span class="sxs-lookup"><span data-stu-id="c6f48-116">1</span></span>|<span data-ttu-id="c6f48-117">程序.</span><span class="sxs-lookup"><span data-stu-id="c6f48-117">Antivirus.</span></span>|
|<span data-ttu-id="c6f48-118">windowsSecurity</span><span class="sxs-lookup"><span data-stu-id="c6f48-118">windowsSecurity</span></span>|<span data-ttu-id="c6f48-119">双面</span><span class="sxs-lookup"><span data-stu-id="c6f48-119">2</span></span>|<span data-ttu-id="c6f48-120">Windows 安全性。</span><span class="sxs-lookup"><span data-stu-id="c6f48-120">Windows Security.</span></span>|
|<span data-ttu-id="c6f48-121">bitLocker</span><span class="sxs-lookup"><span data-stu-id="c6f48-121">bitLocker</span></span>|<span data-ttu-id="c6f48-122">第三章</span><span class="sxs-lookup"><span data-stu-id="c6f48-122">3</span></span>|<span data-ttu-id="c6f48-123">BitLocker.</span><span class="sxs-lookup"><span data-stu-id="c6f48-123">BitLocker.</span></span>|
|<span data-ttu-id="c6f48-124">fileVault</span><span class="sxs-lookup"><span data-stu-id="c6f48-124">fileVault</span></span>|<span data-ttu-id="c6f48-125">4 </span><span class="sxs-lookup"><span data-stu-id="c6f48-125">4</span></span>|<span data-ttu-id="c6f48-126">FileVault.</span><span class="sxs-lookup"><span data-stu-id="c6f48-126">FileVault.</span></span>|
|<span data-ttu-id="c6f48-127">firewall</span><span class="sxs-lookup"><span data-stu-id="c6f48-127">firewall</span></span>|<span data-ttu-id="c6f48-128">5 </span><span class="sxs-lookup"><span data-stu-id="c6f48-128">5</span></span>|<span data-ttu-id="c6f48-129">Firewall.</span><span class="sxs-lookup"><span data-stu-id="c6f48-129">Firewall.</span></span>|
|<span data-ttu-id="c6f48-130">firewallRules</span><span class="sxs-lookup"><span data-stu-id="c6f48-130">firewallRules</span></span>|<span data-ttu-id="c6f48-131">6 </span><span class="sxs-lookup"><span data-stu-id="c6f48-131">6</span></span>|<span data-ttu-id="c6f48-132">防火墙规则。</span><span class="sxs-lookup"><span data-stu-id="c6f48-132">Firewall rules.</span></span>|
|<span data-ttu-id="c6f48-133">endpointDetectionAndResponse</span><span class="sxs-lookup"><span data-stu-id="c6f48-133">endpointDetectionAndResponse</span></span>|<span data-ttu-id="c6f48-134">7 </span><span class="sxs-lookup"><span data-stu-id="c6f48-134">7</span></span>|<span data-ttu-id="c6f48-135">终结点检测和响应。</span><span class="sxs-lookup"><span data-stu-id="c6f48-135">Endpoint detection and response.</span></span>|
|<span data-ttu-id="c6f48-136">deviceControl</span><span class="sxs-lookup"><span data-stu-id="c6f48-136">deviceControl</span></span>|<span data-ttu-id="c6f48-137">8 </span><span class="sxs-lookup"><span data-stu-id="c6f48-137">8</span></span>|<span data-ttu-id="c6f48-138">设备控件。</span><span class="sxs-lookup"><span data-stu-id="c6f48-138">Device control.</span></span>|
|<span data-ttu-id="c6f48-139">appAndBrowserIsolation</span><span class="sxs-lookup"><span data-stu-id="c6f48-139">appAndBrowserIsolation</span></span>|<span data-ttu-id="c6f48-140">9 </span><span class="sxs-lookup"><span data-stu-id="c6f48-140">9</span></span>|<span data-ttu-id="c6f48-141">应用程序和浏览器隔离。</span><span class="sxs-lookup"><span data-stu-id="c6f48-141">App and browser isolation.</span></span>|
|<span data-ttu-id="c6f48-142">exploitProtection</span><span class="sxs-lookup"><span data-stu-id="c6f48-142">exploitProtection</span></span>|<span data-ttu-id="c6f48-143">10  </span><span class="sxs-lookup"><span data-stu-id="c6f48-143">10</span></span>|<span data-ttu-id="c6f48-144">Exploit Protection。</span><span class="sxs-lookup"><span data-stu-id="c6f48-144">Exploit protection.</span></span>|
|<span data-ttu-id="c6f48-145">webProtection</span><span class="sxs-lookup"><span data-stu-id="c6f48-145">webProtection</span></span>|<span data-ttu-id="c6f48-146">11x17</span><span class="sxs-lookup"><span data-stu-id="c6f48-146">11</span></span>|<span data-ttu-id="c6f48-147">Web 保护。</span><span class="sxs-lookup"><span data-stu-id="c6f48-147">Web protection.</span></span>|
|<span data-ttu-id="c6f48-148">applicationControl</span><span class="sxs-lookup"><span data-stu-id="c6f48-148">applicationControl</span></span>|<span data-ttu-id="c6f48-149">12 </span><span class="sxs-lookup"><span data-stu-id="c6f48-149">12</span></span>|<span data-ttu-id="c6f48-150">应用程序控制。</span><span class="sxs-lookup"><span data-stu-id="c6f48-150">Application control.</span></span>|
|<span data-ttu-id="c6f48-151">attackSurfaceReductionRules</span><span class="sxs-lookup"><span data-stu-id="c6f48-151">attackSurfaceReductionRules</span></span>|<span data-ttu-id="c6f48-152">13 </span><span class="sxs-lookup"><span data-stu-id="c6f48-152">13</span></span>|<span data-ttu-id="c6f48-153">攻击面减少规则。</span><span class="sxs-lookup"><span data-stu-id="c6f48-153">Attack surface reduction rules.</span></span>|
|<span data-ttu-id="c6f48-154">accountProtection</span><span class="sxs-lookup"><span data-stu-id="c6f48-154">accountProtection</span></span>|<span data-ttu-id="c6f48-155">14 </span><span class="sxs-lookup"><span data-stu-id="c6f48-155">14</span></span>|<span data-ttu-id="c6f48-156">帐户保护。</span><span class="sxs-lookup"><span data-stu-id="c6f48-156">Account protection.</span></span>|





