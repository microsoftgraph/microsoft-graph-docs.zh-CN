---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1711ad647afabc2b8877bd2f99b049bd1c1dd4e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914281"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="9ff4b-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9ff4b-103">managementAgentType enum type</span></span>

> <span data-ttu-id="9ff4b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ff4b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ff4b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ff4b-107">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-107">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="9ff4b-108">成员</span><span class="sxs-lookup"><span data-stu-id="9ff4b-108">Members</span></span>
|<span data-ttu-id="9ff4b-109">成员</span><span class="sxs-lookup"><span data-stu-id="9ff4b-109">Member</span></span>|<span data-ttu-id="9ff4b-110">值</span><span class="sxs-lookup"><span data-stu-id="9ff4b-110">Value</span></span>|<span data-ttu-id="9ff4b-111">Description</span><span class="sxs-lookup"><span data-stu-id="9ff4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ff4b-112">eas</span><span class="sxs-lookup"><span data-stu-id="9ff4b-112">eas</span></span>|<span data-ttu-id="9ff4b-113">1</span><span class="sxs-lookup"><span data-stu-id="9ff4b-113">1</span></span>|<span data-ttu-id="9ff4b-114">设备管理 Exchange server。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="9ff4b-115">mdm</span><span class="sxs-lookup"><span data-stu-id="9ff4b-115">mdm</span></span>|<span data-ttu-id="9ff4b-116">2</span><span class="sxs-lookup"><span data-stu-id="9ff4b-116">2</span></span>|<span data-ttu-id="9ff4b-117">设备管理由 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="9ff4b-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="9ff4b-118">easMdm</span></span>|<span data-ttu-id="9ff4b-119">3</span><span class="sxs-lookup"><span data-stu-id="9ff4b-119">3</span></span>|<span data-ttu-id="9ff4b-120">设备所管理的 Exchange server 和 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="9ff4b-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="9ff4b-121">intuneClient</span></span>|<span data-ttu-id="9ff4b-122">4</span><span class="sxs-lookup"><span data-stu-id="9ff4b-122">4</span></span>|<span data-ttu-id="9ff4b-123">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-123">Intune client managed.</span></span>|
|<span data-ttu-id="9ff4b-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="9ff4b-124">easIntuneClient</span></span>|<span data-ttu-id="9ff4b-125">5</span><span class="sxs-lookup"><span data-stu-id="9ff4b-125">5</span></span>|<span data-ttu-id="9ff4b-126">设备是 EAS 和 Intune 客户端双托管。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="9ff4b-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="9ff4b-127">configurationManagerClient</span></span>|<span data-ttu-id="9ff4b-128">8</span><span class="sxs-lookup"><span data-stu-id="9ff4b-128">8</span></span>|<span data-ttu-id="9ff4b-129">设备管理由配置管理器中。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="9ff4b-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="9ff4b-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="9ff4b-131">10</span><span class="sxs-lookup"><span data-stu-id="9ff4b-131">10</span></span>|<span data-ttu-id="9ff4b-132">设备所管理的配置管理器和 mdm。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="9ff4b-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="9ff4b-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="9ff4b-134">11</span><span class="sxs-lookup"><span data-stu-id="9ff4b-134">11</span></span>|<span data-ttu-id="9ff4b-135">配置管理器、 MDM 和 Eas 由管理设备。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="9ff4b-136">unknown</span><span class="sxs-lookup"><span data-stu-id="9ff4b-136">unknown</span></span>|<span data-ttu-id="9ff4b-137">16</span><span class="sxs-lookup"><span data-stu-id="9ff4b-137">16</span></span>|<span data-ttu-id="9ff4b-138">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="9ff4b-139">jamf</span><span class="sxs-lookup"><span data-stu-id="9ff4b-139">jamf</span></span>|<span data-ttu-id="9ff4b-140">32</span><span class="sxs-lookup"><span data-stu-id="9ff4b-140">32</span></span>|<span data-ttu-id="9ff4b-141">从 Jamf 获取设备属性。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="9ff4b-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="9ff4b-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="9ff4b-143">64</span><span class="sxs-lookup"><span data-stu-id="9ff4b-143">64</span></span>|<span data-ttu-id="9ff4b-144">由 Google 的 CloudDPC 管理设备。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="9ff4b-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="9ff4b-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="9ff4b-146">258</span><span class="sxs-lookup"><span data-stu-id="9ff4b-146">258</span></span>|<span data-ttu-id="9ff4b-147">由 Microsoft 365 通过 Intune 管理此设备。</span><span class="sxs-lookup"><span data-stu-id="9ff4b-147">This device is managed by Microsoft 365 through Intune.</span></span>|





