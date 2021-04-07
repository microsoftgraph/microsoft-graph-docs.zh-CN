---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 331fd26e009fce708d13f4422c8eef0e6d19d0f8
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612123"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="68765-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="68765-103">managementAgentType enum type</span></span>

<span data-ttu-id="68765-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68765-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68765-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="68765-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68765-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="68765-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68765-107">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="68765-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="68765-108">成员</span><span class="sxs-lookup"><span data-stu-id="68765-108">Members</span></span>
|<span data-ttu-id="68765-109">成员</span><span class="sxs-lookup"><span data-stu-id="68765-109">Member</span></span>|<span data-ttu-id="68765-110">值</span><span class="sxs-lookup"><span data-stu-id="68765-110">Value</span></span>|<span data-ttu-id="68765-111">Description</span><span class="sxs-lookup"><span data-stu-id="68765-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68765-112">eas</span><span class="sxs-lookup"><span data-stu-id="68765-112">eas</span></span>|<span data-ttu-id="68765-113">1</span><span class="sxs-lookup"><span data-stu-id="68765-113">1</span></span>|<span data-ttu-id="68765-114">设备由 Exchange 服务器管理。</span><span class="sxs-lookup"><span data-stu-id="68765-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="68765-115">mdm</span><span class="sxs-lookup"><span data-stu-id="68765-115">mdm</span></span>|<span data-ttu-id="68765-116">2</span><span class="sxs-lookup"><span data-stu-id="68765-116">2</span></span>|<span data-ttu-id="68765-117">设备由 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="68765-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="68765-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="68765-118">easMdm</span></span>|<span data-ttu-id="68765-119">3</span><span class="sxs-lookup"><span data-stu-id="68765-119">3</span></span>|<span data-ttu-id="68765-120">设备由 Exchange 服务器和 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="68765-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="68765-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="68765-121">intuneClient</span></span>|<span data-ttu-id="68765-122">4 </span><span class="sxs-lookup"><span data-stu-id="68765-122">4</span></span>|<span data-ttu-id="68765-123">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="68765-123">Intune client managed.</span></span>|
|<span data-ttu-id="68765-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="68765-124">easIntuneClient</span></span>|<span data-ttu-id="68765-125">5 </span><span class="sxs-lookup"><span data-stu-id="68765-125">5</span></span>|<span data-ttu-id="68765-126">设备是 EAS 和 Intune 客户端双托管设备。</span><span class="sxs-lookup"><span data-stu-id="68765-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="68765-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="68765-127">configurationManagerClient</span></span>|<span data-ttu-id="68765-128">8 </span><span class="sxs-lookup"><span data-stu-id="68765-128">8</span></span>|<span data-ttu-id="68765-129">设备由 Configuration Manager 管理。</span><span class="sxs-lookup"><span data-stu-id="68765-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="68765-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="68765-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="68765-131">10  </span><span class="sxs-lookup"><span data-stu-id="68765-131">10</span></span>|<span data-ttu-id="68765-132">设备由 Configuration Manager 和 MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="68765-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="68765-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="68765-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="68765-134">11</span><span class="sxs-lookup"><span data-stu-id="68765-134">11</span></span>|<span data-ttu-id="68765-135">设备由 Configuration Manager、MDM 和 Eas 管理。</span><span class="sxs-lookup"><span data-stu-id="68765-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="68765-136">unknown</span><span class="sxs-lookup"><span data-stu-id="68765-136">unknown</span></span>|<span data-ttu-id="68765-137">16 </span><span class="sxs-lookup"><span data-stu-id="68765-137">16</span></span>|<span data-ttu-id="68765-138">未知管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="68765-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="68765-139">jamf</span><span class="sxs-lookup"><span data-stu-id="68765-139">jamf</span></span>|<span data-ttu-id="68765-140">32</span><span class="sxs-lookup"><span data-stu-id="68765-140">32</span></span>|<span data-ttu-id="68765-141">设备属性从 Jamf 获取。</span><span class="sxs-lookup"><span data-stu-id="68765-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="68765-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="68765-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="68765-143">64</span><span class="sxs-lookup"><span data-stu-id="68765-143">64</span></span>|<span data-ttu-id="68765-144">设备由 Google 的 CloudDPC 管理。</span><span class="sxs-lookup"><span data-stu-id="68765-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="68765-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="68765-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="68765-146">258</span><span class="sxs-lookup"><span data-stu-id="68765-146">258</span></span>|<span data-ttu-id="68765-147">此设备通过 Intune 由 Microsoft 365 管理。</span><span class="sxs-lookup"><span data-stu-id="68765-147">This device is managed by Microsoft 365 through Intune.</span></span>|




