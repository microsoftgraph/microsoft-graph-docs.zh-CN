---
title: endpointSecurityConfigurationProfileType 枚举类型
description: 终结点安全策略配置文件类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1543584c1b839eedb0c346758f77a906ac41b752
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301072"
---
# <a name="endpointsecurityconfigurationprofiletype-enum-type"></a><span data-ttu-id="db9fc-103">endpointSecurityConfigurationProfileType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="db9fc-103">endpointSecurityConfigurationProfileType enum type</span></span>

<span data-ttu-id="db9fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db9fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db9fc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db9fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db9fc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db9fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db9fc-107">终结点安全策略配置文件类型。</span><span class="sxs-lookup"><span data-stu-id="db9fc-107">The endpoint security policy profile type.</span></span>

## <a name="members"></a><span data-ttu-id="db9fc-108">成员</span><span class="sxs-lookup"><span data-stu-id="db9fc-108">Members</span></span>
|<span data-ttu-id="db9fc-109">成员</span><span class="sxs-lookup"><span data-stu-id="db9fc-109">Member</span></span>|<span data-ttu-id="db9fc-110">值</span><span class="sxs-lookup"><span data-stu-id="db9fc-110">Value</span></span>|<span data-ttu-id="db9fc-111">Description</span><span class="sxs-lookup"><span data-stu-id="db9fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db9fc-112">unknown</span><span class="sxs-lookup"><span data-stu-id="db9fc-112">unknown</span></span>|<span data-ttu-id="db9fc-113">0</span><span class="sxs-lookup"><span data-stu-id="db9fc-113">0</span></span>|<span data-ttu-id="db9fc-114">陌生.</span><span class="sxs-lookup"><span data-stu-id="db9fc-114">Unknown.</span></span>|
|<span data-ttu-id="db9fc-115">程序</span><span class="sxs-lookup"><span data-stu-id="db9fc-115">antivirus</span></span>|<span data-ttu-id="db9fc-116">1</span><span class="sxs-lookup"><span data-stu-id="db9fc-116">1</span></span>|<span data-ttu-id="db9fc-117">程序.</span><span class="sxs-lookup"><span data-stu-id="db9fc-117">Antivirus.</span></span>|
|<span data-ttu-id="db9fc-118">windowsSecurity</span><span class="sxs-lookup"><span data-stu-id="db9fc-118">windowsSecurity</span></span>|<span data-ttu-id="db9fc-119">双面</span><span class="sxs-lookup"><span data-stu-id="db9fc-119">2</span></span>|<span data-ttu-id="db9fc-120">Windows 安全性。</span><span class="sxs-lookup"><span data-stu-id="db9fc-120">Windows Security.</span></span>|
|<span data-ttu-id="db9fc-121">bitLocker</span><span class="sxs-lookup"><span data-stu-id="db9fc-121">bitLocker</span></span>|<span data-ttu-id="db9fc-122">第三章</span><span class="sxs-lookup"><span data-stu-id="db9fc-122">3</span></span>|<span data-ttu-id="db9fc-123">BitLocker.</span><span class="sxs-lookup"><span data-stu-id="db9fc-123">BitLocker.</span></span>|
|<span data-ttu-id="db9fc-124">fileVault</span><span class="sxs-lookup"><span data-stu-id="db9fc-124">fileVault</span></span>|<span data-ttu-id="db9fc-125">4 </span><span class="sxs-lookup"><span data-stu-id="db9fc-125">4</span></span>|<span data-ttu-id="db9fc-126">FileVault.</span><span class="sxs-lookup"><span data-stu-id="db9fc-126">FileVault.</span></span>|
|<span data-ttu-id="db9fc-127">firewall</span><span class="sxs-lookup"><span data-stu-id="db9fc-127">firewall</span></span>|<span data-ttu-id="db9fc-128">5 </span><span class="sxs-lookup"><span data-stu-id="db9fc-128">5</span></span>|<span data-ttu-id="db9fc-129">Firewall.</span><span class="sxs-lookup"><span data-stu-id="db9fc-129">Firewall.</span></span>|
|<span data-ttu-id="db9fc-130">firewallRules</span><span class="sxs-lookup"><span data-stu-id="db9fc-130">firewallRules</span></span>|<span data-ttu-id="db9fc-131">6 </span><span class="sxs-lookup"><span data-stu-id="db9fc-131">6</span></span>|<span data-ttu-id="db9fc-132">防火墙规则。</span><span class="sxs-lookup"><span data-stu-id="db9fc-132">Firewall rules.</span></span>|
|<span data-ttu-id="db9fc-133">endpointDetectionAndResponse</span><span class="sxs-lookup"><span data-stu-id="db9fc-133">endpointDetectionAndResponse</span></span>|<span data-ttu-id="db9fc-134">7 </span><span class="sxs-lookup"><span data-stu-id="db9fc-134">7</span></span>|<span data-ttu-id="db9fc-135">终结点检测和响应。</span><span class="sxs-lookup"><span data-stu-id="db9fc-135">Endpoint detection and response.</span></span>|
|<span data-ttu-id="db9fc-136">deviceControl</span><span class="sxs-lookup"><span data-stu-id="db9fc-136">deviceControl</span></span>|<span data-ttu-id="db9fc-137">8 </span><span class="sxs-lookup"><span data-stu-id="db9fc-137">8</span></span>|<span data-ttu-id="db9fc-138">设备控件。</span><span class="sxs-lookup"><span data-stu-id="db9fc-138">Device control.</span></span>|
|<span data-ttu-id="db9fc-139">appAndBrowserIsolation</span><span class="sxs-lookup"><span data-stu-id="db9fc-139">appAndBrowserIsolation</span></span>|<span data-ttu-id="db9fc-140">9 </span><span class="sxs-lookup"><span data-stu-id="db9fc-140">9</span></span>|<span data-ttu-id="db9fc-141">应用程序和浏览器隔离。</span><span class="sxs-lookup"><span data-stu-id="db9fc-141">App and browser isolation.</span></span>|
|<span data-ttu-id="db9fc-142">exploitProtection</span><span class="sxs-lookup"><span data-stu-id="db9fc-142">exploitProtection</span></span>|<span data-ttu-id="db9fc-143">10  </span><span class="sxs-lookup"><span data-stu-id="db9fc-143">10</span></span>|<span data-ttu-id="db9fc-144">Exploit Protection。</span><span class="sxs-lookup"><span data-stu-id="db9fc-144">Exploit protection.</span></span>|
|<span data-ttu-id="db9fc-145">webProtection</span><span class="sxs-lookup"><span data-stu-id="db9fc-145">webProtection</span></span>|<span data-ttu-id="db9fc-146">11 </span><span class="sxs-lookup"><span data-stu-id="db9fc-146">11</span></span>|<span data-ttu-id="db9fc-147">Web 保护。</span><span class="sxs-lookup"><span data-stu-id="db9fc-147">Web protection.</span></span>|
|<span data-ttu-id="db9fc-148">applicationControl</span><span class="sxs-lookup"><span data-stu-id="db9fc-148">applicationControl</span></span>|<span data-ttu-id="db9fc-149">12 </span><span class="sxs-lookup"><span data-stu-id="db9fc-149">12</span></span>|<span data-ttu-id="db9fc-150">应用程序控制。</span><span class="sxs-lookup"><span data-stu-id="db9fc-150">Application control.</span></span>|
|<span data-ttu-id="db9fc-151">attackSurfaceReductionRules</span><span class="sxs-lookup"><span data-stu-id="db9fc-151">attackSurfaceReductionRules</span></span>|<span data-ttu-id="db9fc-152">13 </span><span class="sxs-lookup"><span data-stu-id="db9fc-152">13</span></span>|<span data-ttu-id="db9fc-153">攻击面减少规则。</span><span class="sxs-lookup"><span data-stu-id="db9fc-153">Attack surface reduction rules.</span></span>|
|<span data-ttu-id="db9fc-154">accountProtection</span><span class="sxs-lookup"><span data-stu-id="db9fc-154">accountProtection</span></span>|<span data-ttu-id="db9fc-155">14 </span><span class="sxs-lookup"><span data-stu-id="db9fc-155">14</span></span>|<span data-ttu-id="db9fc-156">帐户保护。</span><span class="sxs-lookup"><span data-stu-id="db9fc-156">Account protection.</span></span>|




