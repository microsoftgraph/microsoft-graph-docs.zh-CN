---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b8cd60cb8eb1b8ed4ac7bcd8fd321e0dbfdda084
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666336"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="f4241-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f4241-103">managementAgentType enum type</span></span>

<span data-ttu-id="f4241-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4241-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4241-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4241-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4241-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4241-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4241-107">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="f4241-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="f4241-108">成员</span><span class="sxs-lookup"><span data-stu-id="f4241-108">Members</span></span>
|<span data-ttu-id="f4241-109">成员</span><span class="sxs-lookup"><span data-stu-id="f4241-109">Member</span></span>|<span data-ttu-id="f4241-110">值</span><span class="sxs-lookup"><span data-stu-id="f4241-110">Value</span></span>|<span data-ttu-id="f4241-111">说明</span><span class="sxs-lookup"><span data-stu-id="f4241-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4241-112">eas</span><span class="sxs-lookup"><span data-stu-id="f4241-112">eas</span></span>|<span data-ttu-id="f4241-113">1</span><span class="sxs-lookup"><span data-stu-id="f4241-113">1</span></span>|<span data-ttu-id="f4241-114">设备由Exchange管理。</span><span class="sxs-lookup"><span data-stu-id="f4241-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="f4241-115">mdm</span><span class="sxs-lookup"><span data-stu-id="f4241-115">mdm</span></span>|<span data-ttu-id="f4241-116">2</span><span class="sxs-lookup"><span data-stu-id="f4241-116">2</span></span>|<span data-ttu-id="f4241-117">设备由 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="f4241-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="f4241-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="f4241-118">easMdm</span></span>|<span data-ttu-id="f4241-119">3</span><span class="sxs-lookup"><span data-stu-id="f4241-119">3</span></span>|<span data-ttu-id="f4241-120">设备由托管服务器Exchange Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="f4241-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="f4241-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="f4241-121">intuneClient</span></span>|<span data-ttu-id="f4241-122">4 </span><span class="sxs-lookup"><span data-stu-id="f4241-122">4</span></span>|<span data-ttu-id="f4241-123">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="f4241-123">Intune client managed.</span></span>|
|<span data-ttu-id="f4241-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="f4241-124">easIntuneClient</span></span>|<span data-ttu-id="f4241-125">5 </span><span class="sxs-lookup"><span data-stu-id="f4241-125">5</span></span>|<span data-ttu-id="f4241-126">设备是 EAS 和 Intune 客户端双托管设备。</span><span class="sxs-lookup"><span data-stu-id="f4241-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="f4241-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="f4241-127">configurationManagerClient</span></span>|<span data-ttu-id="f4241-128">8 </span><span class="sxs-lookup"><span data-stu-id="f4241-128">8</span></span>|<span data-ttu-id="f4241-129">设备由 Configuration Manager 管理。</span><span class="sxs-lookup"><span data-stu-id="f4241-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="f4241-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="f4241-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="f4241-131">10  </span><span class="sxs-lookup"><span data-stu-id="f4241-131">10</span></span>|<span data-ttu-id="f4241-132">设备由 Configuration Manager 和 MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="f4241-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="f4241-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="f4241-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="f4241-134">11</span><span class="sxs-lookup"><span data-stu-id="f4241-134">11</span></span>|<span data-ttu-id="f4241-135">设备由 Configuration Manager、MDM 和 Eas 管理。</span><span class="sxs-lookup"><span data-stu-id="f4241-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="f4241-136">unknown</span><span class="sxs-lookup"><span data-stu-id="f4241-136">unknown</span></span>|<span data-ttu-id="f4241-137">16 </span><span class="sxs-lookup"><span data-stu-id="f4241-137">16</span></span>|<span data-ttu-id="f4241-138">未知管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="f4241-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="f4241-139">jamf</span><span class="sxs-lookup"><span data-stu-id="f4241-139">jamf</span></span>|<span data-ttu-id="f4241-140">32</span><span class="sxs-lookup"><span data-stu-id="f4241-140">32</span></span>|<span data-ttu-id="f4241-141">设备属性从 Jamf 获取。</span><span class="sxs-lookup"><span data-stu-id="f4241-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="f4241-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="f4241-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="f4241-143">64</span><span class="sxs-lookup"><span data-stu-id="f4241-143">64</span></span>|<span data-ttu-id="f4241-144">设备由 Google 的 CloudDPC 管理。</span><span class="sxs-lookup"><span data-stu-id="f4241-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="f4241-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="f4241-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="f4241-146">258</span><span class="sxs-lookup"><span data-stu-id="f4241-146">258</span></span>|<span data-ttu-id="f4241-147">此设备通过 Intune Microsoft 365管理。</span><span class="sxs-lookup"><span data-stu-id="f4241-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="f4241-148">msSense</span><span class="sxs-lookup"><span data-stu-id="f4241-148">msSense</span></span>|<span data-ttu-id="f4241-149">1024</span><span class="sxs-lookup"><span data-stu-id="f4241-149">1024</span></span>|<span data-ttu-id="f4241-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f4241-150">Not yet documented</span></span>|
|<span data-ttu-id="f4241-151">intuneAosp</span><span class="sxs-lookup"><span data-stu-id="f4241-151">intuneAosp</span></span>|<span data-ttu-id="f4241-152">2048</span><span class="sxs-lookup"><span data-stu-id="f4241-152">2048</span></span>|<span data-ttu-id="f4241-153">此设备由 Intune 的 AOSP MDM (Android 开放源代码Project) 设备</span><span class="sxs-lookup"><span data-stu-id="f4241-153">This device is managed by Intune's MDM for AOSP (Android Open Source Project) devices</span></span>|
|<span data-ttu-id="f4241-154">windowsManagementCloudApi</span><span class="sxs-lookup"><span data-stu-id="f4241-154">windowsManagementCloudApi</span></span>|<span data-ttu-id="f4241-155">512</span><span class="sxs-lookup"><span data-stu-id="f4241-155">512</span></span>|<span data-ttu-id="f4241-156">此设备由 Windows云 API 管理。</span><span class="sxs-lookup"><span data-stu-id="f4241-156">This device is managed by Windows Management Cloud API.</span></span>|



