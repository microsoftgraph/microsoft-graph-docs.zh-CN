---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b8b4f5086ada7351dd41ac165dc600f81dc1fb4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813823"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="57772-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="57772-103">managementAgentType enum type</span></span>

> <span data-ttu-id="57772-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="57772-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57772-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="57772-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57772-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="57772-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57772-107">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="57772-107">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="57772-108">成员</span><span class="sxs-lookup"><span data-stu-id="57772-108">Members</span></span>
|<span data-ttu-id="57772-109">成员</span><span class="sxs-lookup"><span data-stu-id="57772-109">Member</span></span>|<span data-ttu-id="57772-110">值</span><span class="sxs-lookup"><span data-stu-id="57772-110">Value</span></span>|<span data-ttu-id="57772-111">Description</span><span class="sxs-lookup"><span data-stu-id="57772-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57772-112">eas</span><span class="sxs-lookup"><span data-stu-id="57772-112">eas</span></span>|<span data-ttu-id="57772-113">1</span><span class="sxs-lookup"><span data-stu-id="57772-113">1</span></span>|<span data-ttu-id="57772-114">设备管理 Exchange server。</span><span class="sxs-lookup"><span data-stu-id="57772-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="57772-115">mdm</span><span class="sxs-lookup"><span data-stu-id="57772-115">mdm</span></span>|<span data-ttu-id="57772-116">2</span><span class="sxs-lookup"><span data-stu-id="57772-116">2</span></span>|<span data-ttu-id="57772-117">设备管理由 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="57772-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="57772-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="57772-118">easMdm</span></span>|<span data-ttu-id="57772-119">3</span><span class="sxs-lookup"><span data-stu-id="57772-119">3</span></span>|<span data-ttu-id="57772-120">设备所管理的 Exchange server 和 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="57772-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="57772-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="57772-121">intuneClient</span></span>|<span data-ttu-id="57772-122">4</span><span class="sxs-lookup"><span data-stu-id="57772-122">4</span></span>|<span data-ttu-id="57772-123">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="57772-123">Intune client managed.</span></span>|
|<span data-ttu-id="57772-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="57772-124">easIntuneClient</span></span>|<span data-ttu-id="57772-125">5</span><span class="sxs-lookup"><span data-stu-id="57772-125">5</span></span>|<span data-ttu-id="57772-126">设备是 EAS 和 Intune 客户端双托管。</span><span class="sxs-lookup"><span data-stu-id="57772-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="57772-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="57772-127">configurationManagerClient</span></span>|<span data-ttu-id="57772-128">8</span><span class="sxs-lookup"><span data-stu-id="57772-128">8</span></span>|<span data-ttu-id="57772-129">设备管理由配置管理器中。</span><span class="sxs-lookup"><span data-stu-id="57772-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="57772-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="57772-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="57772-131">10</span><span class="sxs-lookup"><span data-stu-id="57772-131">10</span></span>|<span data-ttu-id="57772-132">设备所管理的配置管理器和 mdm。</span><span class="sxs-lookup"><span data-stu-id="57772-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="57772-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="57772-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="57772-134">11</span><span class="sxs-lookup"><span data-stu-id="57772-134">11</span></span>|<span data-ttu-id="57772-135">配置管理器、 MDM 和 Eas 由管理设备。</span><span class="sxs-lookup"><span data-stu-id="57772-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="57772-136">unknown</span><span class="sxs-lookup"><span data-stu-id="57772-136">unknown</span></span>|<span data-ttu-id="57772-137">16</span><span class="sxs-lookup"><span data-stu-id="57772-137">16</span></span>|<span data-ttu-id="57772-138">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="57772-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="57772-139">jamf</span><span class="sxs-lookup"><span data-stu-id="57772-139">jamf</span></span>|<span data-ttu-id="57772-140">32</span><span class="sxs-lookup"><span data-stu-id="57772-140">32</span></span>|<span data-ttu-id="57772-141">从 Jamf 获取设备属性。</span><span class="sxs-lookup"><span data-stu-id="57772-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="57772-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="57772-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="57772-143">64</span><span class="sxs-lookup"><span data-stu-id="57772-143">64</span></span>|<span data-ttu-id="57772-144">由 Google 的 CloudDPC 管理设备。</span><span class="sxs-lookup"><span data-stu-id="57772-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="57772-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="57772-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="57772-146">258</span><span class="sxs-lookup"><span data-stu-id="57772-146">258</span></span>|<span data-ttu-id="57772-147">由 Microsoft 365 通过 Intune 管理此设备。</span><span class="sxs-lookup"><span data-stu-id="57772-147">This device is managed by Microsoft 365 through Intune.</span></span>|





