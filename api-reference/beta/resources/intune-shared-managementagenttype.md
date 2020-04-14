---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 34783f2c586e192d62cdeb0018b82e2df100c958
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466241"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="11902-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="11902-103">managementAgentType enum type</span></span>

<span data-ttu-id="11902-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11902-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11902-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11902-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11902-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11902-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11902-107">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="11902-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="11902-108">成员</span><span class="sxs-lookup"><span data-stu-id="11902-108">Members</span></span>
|<span data-ttu-id="11902-109">成员</span><span class="sxs-lookup"><span data-stu-id="11902-109">Member</span></span>|<span data-ttu-id="11902-110">值</span><span class="sxs-lookup"><span data-stu-id="11902-110">Value</span></span>|<span data-ttu-id="11902-111">说明</span><span class="sxs-lookup"><span data-stu-id="11902-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11902-112">符合</span><span class="sxs-lookup"><span data-stu-id="11902-112">eas</span></span>|<span data-ttu-id="11902-113">1</span><span class="sxs-lookup"><span data-stu-id="11902-113">1</span></span>|<span data-ttu-id="11902-114">设备由 Exchange server 管理。</span><span class="sxs-lookup"><span data-stu-id="11902-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="11902-115">mdm</span><span class="sxs-lookup"><span data-stu-id="11902-115">mdm</span></span>|<span data-ttu-id="11902-116">双面</span><span class="sxs-lookup"><span data-stu-id="11902-116">2</span></span>|<span data-ttu-id="11902-117">设备由 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="11902-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="11902-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="11902-118">easMdm</span></span>|<span data-ttu-id="11902-119">第三章</span><span class="sxs-lookup"><span data-stu-id="11902-119">3</span></span>|<span data-ttu-id="11902-120">设备由 Exchange server 和 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="11902-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="11902-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="11902-121">intuneClient</span></span>|<span data-ttu-id="11902-122">4 </span><span class="sxs-lookup"><span data-stu-id="11902-122">4</span></span>|<span data-ttu-id="11902-123">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="11902-123">Intune client managed.</span></span>|
|<span data-ttu-id="11902-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="11902-124">easIntuneClient</span></span>|<span data-ttu-id="11902-125">5 </span><span class="sxs-lookup"><span data-stu-id="11902-125">5</span></span>|<span data-ttu-id="11902-126">设备为 EAS 和 Intune 客户端双重托管。</span><span class="sxs-lookup"><span data-stu-id="11902-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="11902-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="11902-127">configurationManagerClient</span></span>|<span data-ttu-id="11902-128">8 </span><span class="sxs-lookup"><span data-stu-id="11902-128">8</span></span>|<span data-ttu-id="11902-129">设备由配置管理器管理。</span><span class="sxs-lookup"><span data-stu-id="11902-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="11902-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="11902-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="11902-131">10 </span><span class="sxs-lookup"><span data-stu-id="11902-131">10</span></span>|<span data-ttu-id="11902-132">设备由 Configuration Manager 和 MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="11902-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="11902-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="11902-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="11902-134">11x17</span><span class="sxs-lookup"><span data-stu-id="11902-134">11</span></span>|<span data-ttu-id="11902-135">设备由 Configuration Manager、MDM 和 Eas 管理。</span><span class="sxs-lookup"><span data-stu-id="11902-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="11902-136">unknown</span><span class="sxs-lookup"><span data-stu-id="11902-136">unknown</span></span>|<span data-ttu-id="11902-137">16 </span><span class="sxs-lookup"><span data-stu-id="11902-137">16</span></span>|<span data-ttu-id="11902-138">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="11902-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="11902-139">jamf</span><span class="sxs-lookup"><span data-stu-id="11902-139">jamf</span></span>|<span data-ttu-id="11902-140">32</span><span class="sxs-lookup"><span data-stu-id="11902-140">32</span></span>|<span data-ttu-id="11902-141">设备属性是从 Jamf 中提取的。</span><span class="sxs-lookup"><span data-stu-id="11902-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="11902-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="11902-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="11902-143">64</span><span class="sxs-lookup"><span data-stu-id="11902-143">64</span></span>|<span data-ttu-id="11902-144">设备由 Google 的 CloudDPC 管理。</span><span class="sxs-lookup"><span data-stu-id="11902-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="11902-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="11902-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="11902-146">258</span><span class="sxs-lookup"><span data-stu-id="11902-146">258</span></span>|<span data-ttu-id="11902-147">此设备由 Microsoft 365 到 Intune 管理。</span><span class="sxs-lookup"><span data-stu-id="11902-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="11902-148">windowsManagementCloudApi</span><span class="sxs-lookup"><span data-stu-id="11902-148">windowsManagementCloudApi</span></span>|<span data-ttu-id="11902-149">512</span><span class="sxs-lookup"><span data-stu-id="11902-149">512</span></span>|<span data-ttu-id="11902-150">此设备由 Windows Management 云 API 管理。</span><span class="sxs-lookup"><span data-stu-id="11902-150">This device is managed by Windows Management Cloud API.</span></span>|



