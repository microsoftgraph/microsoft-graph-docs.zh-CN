---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf8a40b8d6951c13da49766430fdd7fb303cbba0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521297"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="a1654-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a1654-103">managementAgentType enum type</span></span>

> <span data-ttu-id="a1654-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1654-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1654-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1654-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1654-106">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="a1654-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="a1654-107">成员</span><span class="sxs-lookup"><span data-stu-id="a1654-107">Members</span></span>
|<span data-ttu-id="a1654-108">成员</span><span class="sxs-lookup"><span data-stu-id="a1654-108">Member</span></span>|<span data-ttu-id="a1654-109">值</span><span class="sxs-lookup"><span data-stu-id="a1654-109">Value</span></span>|<span data-ttu-id="a1654-110">说明</span><span class="sxs-lookup"><span data-stu-id="a1654-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1654-111">符合</span><span class="sxs-lookup"><span data-stu-id="a1654-111">eas</span></span>|<span data-ttu-id="a1654-112">1</span><span class="sxs-lookup"><span data-stu-id="a1654-112">1</span></span>|<span data-ttu-id="a1654-113">设备由 Exchange server 管理。</span><span class="sxs-lookup"><span data-stu-id="a1654-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="a1654-114">mdm</span><span class="sxs-lookup"><span data-stu-id="a1654-114">mdm</span></span>|<span data-ttu-id="a1654-115">2 </span><span class="sxs-lookup"><span data-stu-id="a1654-115">2</span></span>|<span data-ttu-id="a1654-116">设备由 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="a1654-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="a1654-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="a1654-117">easMdm</span></span>|<span data-ttu-id="a1654-118">3 </span><span class="sxs-lookup"><span data-stu-id="a1654-118">3</span></span>|<span data-ttu-id="a1654-119">设备由 Exchange server 和 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="a1654-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="a1654-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="a1654-120">intuneClient</span></span>|<span data-ttu-id="a1654-121">4 </span><span class="sxs-lookup"><span data-stu-id="a1654-121">4</span></span>|<span data-ttu-id="a1654-122">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="a1654-122">Intune client managed.</span></span>|
|<span data-ttu-id="a1654-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="a1654-123">easIntuneClient</span></span>|<span data-ttu-id="a1654-124">5 </span><span class="sxs-lookup"><span data-stu-id="a1654-124">5</span></span>|<span data-ttu-id="a1654-125">设备为 EAS 和 Intune 客户端双重托管。</span><span class="sxs-lookup"><span data-stu-id="a1654-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="a1654-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="a1654-126">configurationManagerClient</span></span>|<span data-ttu-id="a1654-127">8 </span><span class="sxs-lookup"><span data-stu-id="a1654-127">8</span></span>|<span data-ttu-id="a1654-128">设备由配置管理器管理。</span><span class="sxs-lookup"><span data-stu-id="a1654-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="a1654-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="a1654-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="a1654-130">10 </span><span class="sxs-lookup"><span data-stu-id="a1654-130">10</span></span>|<span data-ttu-id="a1654-131">设备由 Configuration Manager 和 MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="a1654-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="a1654-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="a1654-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="a1654-133">11 </span><span class="sxs-lookup"><span data-stu-id="a1654-133">11</span></span>|<span data-ttu-id="a1654-134">设备由 Configuration Manager、MDM 和 Eas 管理。</span><span class="sxs-lookup"><span data-stu-id="a1654-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="a1654-135">unknown</span><span class="sxs-lookup"><span data-stu-id="a1654-135">unknown</span></span>|<span data-ttu-id="a1654-136">16 </span><span class="sxs-lookup"><span data-stu-id="a1654-136">16</span></span>|<span data-ttu-id="a1654-137">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="a1654-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="a1654-138">jamf</span><span class="sxs-lookup"><span data-stu-id="a1654-138">jamf</span></span>|<span data-ttu-id="a1654-139">32</span><span class="sxs-lookup"><span data-stu-id="a1654-139">32</span></span>|<span data-ttu-id="a1654-140">设备属性是从 Jamf 中提取的。</span><span class="sxs-lookup"><span data-stu-id="a1654-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="a1654-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="a1654-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="a1654-142">64</span><span class="sxs-lookup"><span data-stu-id="a1654-142">64</span></span>|<span data-ttu-id="a1654-143">设备由 Google 的 CloudDPC 管理。</span><span class="sxs-lookup"><span data-stu-id="a1654-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="a1654-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="a1654-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="a1654-145">258</span><span class="sxs-lookup"><span data-stu-id="a1654-145">258</span></span>|<span data-ttu-id="a1654-146">此设备由 Microsoft 365 到 Intune 管理。</span><span class="sxs-lookup"><span data-stu-id="a1654-146">This device is managed by Microsoft 365 through Intune.</span></span>|





