---
title: endpointSecurityConfigurationProfileType 枚举类型
description: 终结点安全策略配置文件类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5b3f3340a9e3aa5aa211b39176e9fe43d74b8bf8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993642"
---
# <a name="endpointsecurityconfigurationprofiletype-enum-type"></a><span data-ttu-id="d6d75-103">endpointSecurityConfigurationProfileType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d6d75-103">endpointSecurityConfigurationProfileType enum type</span></span>

<span data-ttu-id="d6d75-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6d75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6d75-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6d75-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6d75-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6d75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6d75-107">终结点安全策略配置文件类型。</span><span class="sxs-lookup"><span data-stu-id="d6d75-107">The endpoint security policy profile type.</span></span>

## <a name="members"></a><span data-ttu-id="d6d75-108">成员</span><span class="sxs-lookup"><span data-stu-id="d6d75-108">Members</span></span>
|<span data-ttu-id="d6d75-109">成员</span><span class="sxs-lookup"><span data-stu-id="d6d75-109">Member</span></span>|<span data-ttu-id="d6d75-110">值</span><span class="sxs-lookup"><span data-stu-id="d6d75-110">Value</span></span>|<span data-ttu-id="d6d75-111">说明</span><span class="sxs-lookup"><span data-stu-id="d6d75-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6d75-112">unknown</span><span class="sxs-lookup"><span data-stu-id="d6d75-112">unknown</span></span>|<span data-ttu-id="d6d75-113">0</span><span class="sxs-lookup"><span data-stu-id="d6d75-113">0</span></span>|<span data-ttu-id="d6d75-114">陌生.</span><span class="sxs-lookup"><span data-stu-id="d6d75-114">Unknown.</span></span>|
|<span data-ttu-id="d6d75-115">程序</span><span class="sxs-lookup"><span data-stu-id="d6d75-115">antivirus</span></span>|<span data-ttu-id="d6d75-116">1 </span><span class="sxs-lookup"><span data-stu-id="d6d75-116">1</span></span>|<span data-ttu-id="d6d75-117">程序.</span><span class="sxs-lookup"><span data-stu-id="d6d75-117">Antivirus.</span></span>|
|<span data-ttu-id="d6d75-118">windowsSecurity</span><span class="sxs-lookup"><span data-stu-id="d6d75-118">windowsSecurity</span></span>|<span data-ttu-id="d6d75-119">2 </span><span class="sxs-lookup"><span data-stu-id="d6d75-119">2</span></span>|<span data-ttu-id="d6d75-120">Windows 安全性。</span><span class="sxs-lookup"><span data-stu-id="d6d75-120">Windows Security.</span></span>|
|<span data-ttu-id="d6d75-121">bitLocker</span><span class="sxs-lookup"><span data-stu-id="d6d75-121">bitLocker</span></span>|<span data-ttu-id="d6d75-122">第三章</span><span class="sxs-lookup"><span data-stu-id="d6d75-122">3</span></span>|<span data-ttu-id="d6d75-123">BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d6d75-123">BitLocker.</span></span>|
|<span data-ttu-id="d6d75-124">fileVault</span><span class="sxs-lookup"><span data-stu-id="d6d75-124">fileVault</span></span>|<span data-ttu-id="d6d75-125">4 </span><span class="sxs-lookup"><span data-stu-id="d6d75-125">4</span></span>|<span data-ttu-id="d6d75-126">FileVault.</span><span class="sxs-lookup"><span data-stu-id="d6d75-126">FileVault.</span></span>|
|<span data-ttu-id="d6d75-127">firewall</span><span class="sxs-lookup"><span data-stu-id="d6d75-127">firewall</span></span>|<span data-ttu-id="d6d75-128">5 </span><span class="sxs-lookup"><span data-stu-id="d6d75-128">5</span></span>|<span data-ttu-id="d6d75-129">Firewall.</span><span class="sxs-lookup"><span data-stu-id="d6d75-129">Firewall.</span></span>|
|<span data-ttu-id="d6d75-130">firewallRules</span><span class="sxs-lookup"><span data-stu-id="d6d75-130">firewallRules</span></span>|<span data-ttu-id="d6d75-131">6 </span><span class="sxs-lookup"><span data-stu-id="d6d75-131">6</span></span>|<span data-ttu-id="d6d75-132">防火墙规则。</span><span class="sxs-lookup"><span data-stu-id="d6d75-132">Firewall rules.</span></span>|
|<span data-ttu-id="d6d75-133">endpointDetectionAndResponse</span><span class="sxs-lookup"><span data-stu-id="d6d75-133">endpointDetectionAndResponse</span></span>|<span data-ttu-id="d6d75-134">7 </span><span class="sxs-lookup"><span data-stu-id="d6d75-134">7</span></span>|<span data-ttu-id="d6d75-135">终结点检测和响应。</span><span class="sxs-lookup"><span data-stu-id="d6d75-135">Endpoint detection and response.</span></span>|
|<span data-ttu-id="d6d75-136">deviceControl</span><span class="sxs-lookup"><span data-stu-id="d6d75-136">deviceControl</span></span>|<span data-ttu-id="d6d75-137">8 </span><span class="sxs-lookup"><span data-stu-id="d6d75-137">8</span></span>|<span data-ttu-id="d6d75-138">设备控件。</span><span class="sxs-lookup"><span data-stu-id="d6d75-138">Device control.</span></span>|
|<span data-ttu-id="d6d75-139">appAndBrowserIsolation</span><span class="sxs-lookup"><span data-stu-id="d6d75-139">appAndBrowserIsolation</span></span>|<span data-ttu-id="d6d75-140">9 </span><span class="sxs-lookup"><span data-stu-id="d6d75-140">9</span></span>|<span data-ttu-id="d6d75-141">应用程序和浏览器隔离。</span><span class="sxs-lookup"><span data-stu-id="d6d75-141">App and browser isolation.</span></span>|
|<span data-ttu-id="d6d75-142">exploitProtection</span><span class="sxs-lookup"><span data-stu-id="d6d75-142">exploitProtection</span></span>|<span data-ttu-id="d6d75-143">10 </span><span class="sxs-lookup"><span data-stu-id="d6d75-143">10</span></span>|<span data-ttu-id="d6d75-144">Exploit Protection。</span><span class="sxs-lookup"><span data-stu-id="d6d75-144">Exploit protection.</span></span>|
|<span data-ttu-id="d6d75-145">webProtection</span><span class="sxs-lookup"><span data-stu-id="d6d75-145">webProtection</span></span>|<span data-ttu-id="d6d75-146">11 </span><span class="sxs-lookup"><span data-stu-id="d6d75-146">11</span></span>|<span data-ttu-id="d6d75-147">Web 保护。</span><span class="sxs-lookup"><span data-stu-id="d6d75-147">Web protection.</span></span>|
|<span data-ttu-id="d6d75-148">applicationControl</span><span class="sxs-lookup"><span data-stu-id="d6d75-148">applicationControl</span></span>|<span data-ttu-id="d6d75-149">12 </span><span class="sxs-lookup"><span data-stu-id="d6d75-149">12</span></span>|<span data-ttu-id="d6d75-150">应用程序控制。</span><span class="sxs-lookup"><span data-stu-id="d6d75-150">Application control.</span></span>|
|<span data-ttu-id="d6d75-151">attackSurfaceReductionRules</span><span class="sxs-lookup"><span data-stu-id="d6d75-151">attackSurfaceReductionRules</span></span>|<span data-ttu-id="d6d75-152">13 </span><span class="sxs-lookup"><span data-stu-id="d6d75-152">13</span></span>|<span data-ttu-id="d6d75-153">攻击面减少规则。</span><span class="sxs-lookup"><span data-stu-id="d6d75-153">Attack surface reduction rules.</span></span>|
|<span data-ttu-id="d6d75-154">accountProtection</span><span class="sxs-lookup"><span data-stu-id="d6d75-154">accountProtection</span></span>|<span data-ttu-id="d6d75-155">14 </span><span class="sxs-lookup"><span data-stu-id="d6d75-155">14</span></span>|<span data-ttu-id="d6d75-156">帐户保护。</span><span class="sxs-lookup"><span data-stu-id="d6d75-156">Account protection.</span></span>|






