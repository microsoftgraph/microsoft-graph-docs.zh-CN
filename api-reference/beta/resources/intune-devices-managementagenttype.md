---
title: managementAgentType 枚举类型
description: 管理代理类型。
ms.openlocfilehash: 334a89c3c8a5934f491626b0956a4532cdf76de0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047774"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="770f4-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="770f4-103">managementAgentType enum type</span></span>

> <span data-ttu-id="770f4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="770f4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="770f4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="770f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="770f4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="770f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="770f4-107">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="770f4-107">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="770f4-108">成员</span><span class="sxs-lookup"><span data-stu-id="770f4-108">Members</span></span>
|<span data-ttu-id="770f4-109">成员</span><span class="sxs-lookup"><span data-stu-id="770f4-109">Member</span></span>|<span data-ttu-id="770f4-110">值</span><span class="sxs-lookup"><span data-stu-id="770f4-110">Value</span></span>|<span data-ttu-id="770f4-111">说明</span><span class="sxs-lookup"><span data-stu-id="770f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="770f4-112">eas</span><span class="sxs-lookup"><span data-stu-id="770f4-112">eas</span></span>|<span data-ttu-id="770f4-113">1</span><span class="sxs-lookup"><span data-stu-id="770f4-113">1</span></span>|<span data-ttu-id="770f4-114">设备管理 Exchange server。</span><span class="sxs-lookup"><span data-stu-id="770f4-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="770f4-115">mdm</span><span class="sxs-lookup"><span data-stu-id="770f4-115">mdm</span></span>|<span data-ttu-id="770f4-116">2</span><span class="sxs-lookup"><span data-stu-id="770f4-116">2</span></span>|<span data-ttu-id="770f4-117">设备管理由 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="770f4-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="770f4-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="770f4-118">easMdm</span></span>|<span data-ttu-id="770f4-119">3</span><span class="sxs-lookup"><span data-stu-id="770f4-119">3</span></span>|<span data-ttu-id="770f4-120">设备所管理的 Exchange server 和 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="770f4-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="770f4-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="770f4-121">intuneClient</span></span>|<span data-ttu-id="770f4-122">4</span><span class="sxs-lookup"><span data-stu-id="770f4-122">4</span></span>|<span data-ttu-id="770f4-123">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="770f4-123">Intune client managed.</span></span>|
|<span data-ttu-id="770f4-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="770f4-124">easIntuneClient</span></span>|<span data-ttu-id="770f4-125">5</span><span class="sxs-lookup"><span data-stu-id="770f4-125">5</span></span>|<span data-ttu-id="770f4-126">设备是 EAS 和 Intune 客户端双托管。</span><span class="sxs-lookup"><span data-stu-id="770f4-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="770f4-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="770f4-127">configurationManagerClient</span></span>|<span data-ttu-id="770f4-128">8</span><span class="sxs-lookup"><span data-stu-id="770f4-128">8</span></span>|<span data-ttu-id="770f4-129">设备管理由配置管理器中。</span><span class="sxs-lookup"><span data-stu-id="770f4-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="770f4-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="770f4-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="770f4-131">10</span><span class="sxs-lookup"><span data-stu-id="770f4-131">10</span></span>|<span data-ttu-id="770f4-132">设备所管理的配置管理器和 mdm。</span><span class="sxs-lookup"><span data-stu-id="770f4-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="770f4-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="770f4-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="770f4-134">11</span><span class="sxs-lookup"><span data-stu-id="770f4-134">11</span></span>|<span data-ttu-id="770f4-135">配置管理器、 MDM 和 Eas 由管理设备。</span><span class="sxs-lookup"><span data-stu-id="770f4-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="770f4-136">unknown</span><span class="sxs-lookup"><span data-stu-id="770f4-136">unknown</span></span>|<span data-ttu-id="770f4-137">16</span><span class="sxs-lookup"><span data-stu-id="770f4-137">16</span></span>|<span data-ttu-id="770f4-138">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="770f4-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="770f4-139">jamf</span><span class="sxs-lookup"><span data-stu-id="770f4-139">jamf</span></span>|<span data-ttu-id="770f4-140">32</span><span class="sxs-lookup"><span data-stu-id="770f4-140">32</span></span>|<span data-ttu-id="770f4-141">从 Jamf 获取设备属性。</span><span class="sxs-lookup"><span data-stu-id="770f4-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="770f4-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="770f4-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="770f4-143">64</span><span class="sxs-lookup"><span data-stu-id="770f4-143">64</span></span>|<span data-ttu-id="770f4-144">由 Google 的 CloudDPC 管理设备。</span><span class="sxs-lookup"><span data-stu-id="770f4-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="770f4-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="770f4-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="770f4-146">258</span><span class="sxs-lookup"><span data-stu-id="770f4-146">258</span></span>|<span data-ttu-id="770f4-147">由 Microsoft 365 通过 Intune 管理此设备。</span><span class="sxs-lookup"><span data-stu-id="770f4-147">This device is managed by Microsoft 365 through Intune.</span></span>|





