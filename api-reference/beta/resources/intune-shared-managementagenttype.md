---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 282915b085107d5367a0b7f8bd8f4f3ea84b7c23
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258939"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="d33f3-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d33f3-103">managementAgentType enum type</span></span>

<span data-ttu-id="d33f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d33f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d33f3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d33f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d33f3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d33f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d33f3-107">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="d33f3-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="d33f3-108">成员</span><span class="sxs-lookup"><span data-stu-id="d33f3-108">Members</span></span>
|<span data-ttu-id="d33f3-109">成员</span><span class="sxs-lookup"><span data-stu-id="d33f3-109">Member</span></span>|<span data-ttu-id="d33f3-110">值</span><span class="sxs-lookup"><span data-stu-id="d33f3-110">Value</span></span>|<span data-ttu-id="d33f3-111">说明</span><span class="sxs-lookup"><span data-stu-id="d33f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d33f3-112">符合</span><span class="sxs-lookup"><span data-stu-id="d33f3-112">eas</span></span>|<span data-ttu-id="d33f3-113">1</span><span class="sxs-lookup"><span data-stu-id="d33f3-113">1</span></span>|<span data-ttu-id="d33f3-114">设备由 Exchange server 管理。</span><span class="sxs-lookup"><span data-stu-id="d33f3-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="d33f3-115">mdm</span><span class="sxs-lookup"><span data-stu-id="d33f3-115">mdm</span></span>|<span data-ttu-id="d33f3-116">双面</span><span class="sxs-lookup"><span data-stu-id="d33f3-116">2</span></span>|<span data-ttu-id="d33f3-117">设备由 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="d33f3-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="d33f3-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="d33f3-118">easMdm</span></span>|<span data-ttu-id="d33f3-119">第三章</span><span class="sxs-lookup"><span data-stu-id="d33f3-119">3</span></span>|<span data-ttu-id="d33f3-120">设备由 Exchange server 和 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="d33f3-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="d33f3-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="d33f3-121">intuneClient</span></span>|<span data-ttu-id="d33f3-122">4 </span><span class="sxs-lookup"><span data-stu-id="d33f3-122">4</span></span>|<span data-ttu-id="d33f3-123">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="d33f3-123">Intune client managed.</span></span>|
|<span data-ttu-id="d33f3-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="d33f3-124">easIntuneClient</span></span>|<span data-ttu-id="d33f3-125">5 </span><span class="sxs-lookup"><span data-stu-id="d33f3-125">5</span></span>|<span data-ttu-id="d33f3-126">设备为 EAS 和 Intune 客户端双重托管。</span><span class="sxs-lookup"><span data-stu-id="d33f3-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="d33f3-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="d33f3-127">configurationManagerClient</span></span>|<span data-ttu-id="d33f3-128">8 </span><span class="sxs-lookup"><span data-stu-id="d33f3-128">8</span></span>|<span data-ttu-id="d33f3-129">设备由配置管理器管理。</span><span class="sxs-lookup"><span data-stu-id="d33f3-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="d33f3-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="d33f3-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="d33f3-131">10  </span><span class="sxs-lookup"><span data-stu-id="d33f3-131">10</span></span>|<span data-ttu-id="d33f3-132">设备由 Configuration Manager 和 MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="d33f3-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="d33f3-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="d33f3-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="d33f3-134">11 </span><span class="sxs-lookup"><span data-stu-id="d33f3-134">11</span></span>|<span data-ttu-id="d33f3-135">设备由 Configuration Manager、MDM 和 Eas 管理。</span><span class="sxs-lookup"><span data-stu-id="d33f3-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="d33f3-136">unknown</span><span class="sxs-lookup"><span data-stu-id="d33f3-136">unknown</span></span>|<span data-ttu-id="d33f3-137">16 </span><span class="sxs-lookup"><span data-stu-id="d33f3-137">16</span></span>|<span data-ttu-id="d33f3-138">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="d33f3-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="d33f3-139">jamf</span><span class="sxs-lookup"><span data-stu-id="d33f3-139">jamf</span></span>|<span data-ttu-id="d33f3-140">32</span><span class="sxs-lookup"><span data-stu-id="d33f3-140">32</span></span>|<span data-ttu-id="d33f3-141">设备属性是从 Jamf 中提取的。</span><span class="sxs-lookup"><span data-stu-id="d33f3-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="d33f3-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="d33f3-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="d33f3-143">64</span><span class="sxs-lookup"><span data-stu-id="d33f3-143">64</span></span>|<span data-ttu-id="d33f3-144">设备由 Google 的 CloudDPC 管理。</span><span class="sxs-lookup"><span data-stu-id="d33f3-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="d33f3-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="d33f3-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="d33f3-146">258</span><span class="sxs-lookup"><span data-stu-id="d33f3-146">258</span></span>|<span data-ttu-id="d33f3-147">此设备由 Microsoft 365 到 Intune 管理。</span><span class="sxs-lookup"><span data-stu-id="d33f3-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="d33f3-148">windowsManagementCloudApi</span><span class="sxs-lookup"><span data-stu-id="d33f3-148">windowsManagementCloudApi</span></span>|<span data-ttu-id="d33f3-149">512</span><span class="sxs-lookup"><span data-stu-id="d33f3-149">512</span></span>|<span data-ttu-id="d33f3-150">此设备由 Windows Management 云 API 管理。</span><span class="sxs-lookup"><span data-stu-id="d33f3-150">This device is managed by Windows Management Cloud API.</span></span>|




