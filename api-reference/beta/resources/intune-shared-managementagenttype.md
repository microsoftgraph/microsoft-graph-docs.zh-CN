---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e769cd3f270a8ca1d00b6272a90154b925cc771d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48681955"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="6913e-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6913e-103">managementAgentType enum type</span></span>

<span data-ttu-id="6913e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6913e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6913e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6913e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6913e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6913e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6913e-107">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="6913e-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="6913e-108">成员</span><span class="sxs-lookup"><span data-stu-id="6913e-108">Members</span></span>
|<span data-ttu-id="6913e-109">成员</span><span class="sxs-lookup"><span data-stu-id="6913e-109">Member</span></span>|<span data-ttu-id="6913e-110">值</span><span class="sxs-lookup"><span data-stu-id="6913e-110">Value</span></span>|<span data-ttu-id="6913e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6913e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6913e-112">符合</span><span class="sxs-lookup"><span data-stu-id="6913e-112">eas</span></span>|<span data-ttu-id="6913e-113">1</span><span class="sxs-lookup"><span data-stu-id="6913e-113">1</span></span>|<span data-ttu-id="6913e-114">设备由 Exchange server 管理。</span><span class="sxs-lookup"><span data-stu-id="6913e-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="6913e-115">mdm</span><span class="sxs-lookup"><span data-stu-id="6913e-115">mdm</span></span>|<span data-ttu-id="6913e-116">双面</span><span class="sxs-lookup"><span data-stu-id="6913e-116">2</span></span>|<span data-ttu-id="6913e-117">设备由 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="6913e-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="6913e-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="6913e-118">easMdm</span></span>|<span data-ttu-id="6913e-119">第三章</span><span class="sxs-lookup"><span data-stu-id="6913e-119">3</span></span>|<span data-ttu-id="6913e-120">设备由 Exchange server 和 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="6913e-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="6913e-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="6913e-121">intuneClient</span></span>|<span data-ttu-id="6913e-122">4 </span><span class="sxs-lookup"><span data-stu-id="6913e-122">4</span></span>|<span data-ttu-id="6913e-123">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="6913e-123">Intune client managed.</span></span>|
|<span data-ttu-id="6913e-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="6913e-124">easIntuneClient</span></span>|<span data-ttu-id="6913e-125">5 </span><span class="sxs-lookup"><span data-stu-id="6913e-125">5</span></span>|<span data-ttu-id="6913e-126">设备为 EAS 和 Intune 客户端双重托管。</span><span class="sxs-lookup"><span data-stu-id="6913e-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="6913e-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="6913e-127">configurationManagerClient</span></span>|<span data-ttu-id="6913e-128">8 </span><span class="sxs-lookup"><span data-stu-id="6913e-128">8</span></span>|<span data-ttu-id="6913e-129">设备由配置管理器管理。</span><span class="sxs-lookup"><span data-stu-id="6913e-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="6913e-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="6913e-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="6913e-131">10  </span><span class="sxs-lookup"><span data-stu-id="6913e-131">10</span></span>|<span data-ttu-id="6913e-132">设备由 Configuration Manager 和 MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="6913e-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="6913e-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="6913e-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="6913e-134">11x17</span><span class="sxs-lookup"><span data-stu-id="6913e-134">11</span></span>|<span data-ttu-id="6913e-135">设备由 Configuration Manager、MDM 和 Eas 管理。</span><span class="sxs-lookup"><span data-stu-id="6913e-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="6913e-136">unknown</span><span class="sxs-lookup"><span data-stu-id="6913e-136">unknown</span></span>|<span data-ttu-id="6913e-137">16 </span><span class="sxs-lookup"><span data-stu-id="6913e-137">16</span></span>|<span data-ttu-id="6913e-138">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="6913e-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="6913e-139">jamf</span><span class="sxs-lookup"><span data-stu-id="6913e-139">jamf</span></span>|<span data-ttu-id="6913e-140">32</span><span class="sxs-lookup"><span data-stu-id="6913e-140">32</span></span>|<span data-ttu-id="6913e-141">设备属性是从 Jamf 中提取的。</span><span class="sxs-lookup"><span data-stu-id="6913e-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="6913e-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="6913e-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="6913e-143">64</span><span class="sxs-lookup"><span data-stu-id="6913e-143">64</span></span>|<span data-ttu-id="6913e-144">设备由 Google 的 CloudDPC 管理。</span><span class="sxs-lookup"><span data-stu-id="6913e-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="6913e-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="6913e-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="6913e-146">258</span><span class="sxs-lookup"><span data-stu-id="6913e-146">258</span></span>|<span data-ttu-id="6913e-147">此设备由 Microsoft 365 到 Intune 管理。</span><span class="sxs-lookup"><span data-stu-id="6913e-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="6913e-148">windowsManagementCloudApi</span><span class="sxs-lookup"><span data-stu-id="6913e-148">windowsManagementCloudApi</span></span>|<span data-ttu-id="6913e-149">512</span><span class="sxs-lookup"><span data-stu-id="6913e-149">512</span></span>|<span data-ttu-id="6913e-150">此设备由 Windows Management 云 API 管理。</span><span class="sxs-lookup"><span data-stu-id="6913e-150">This device is managed by Windows Management Cloud API.</span></span>|





