---
title: managementAgentType 枚举类型
description: 管理代理类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9c42d4ea4a5114bc42966891e4cd60ea87ca303e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401003"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="6439a-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6439a-103">managementAgentType enum type</span></span>

> <span data-ttu-id="6439a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6439a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6439a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6439a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6439a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6439a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6439a-107">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="6439a-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="6439a-108">成员</span><span class="sxs-lookup"><span data-stu-id="6439a-108">Members</span></span>
|<span data-ttu-id="6439a-109">成员</span><span class="sxs-lookup"><span data-stu-id="6439a-109">Member</span></span>|<span data-ttu-id="6439a-110">值</span><span class="sxs-lookup"><span data-stu-id="6439a-110">Value</span></span>|<span data-ttu-id="6439a-111">说明</span><span class="sxs-lookup"><span data-stu-id="6439a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6439a-112">eas</span><span class="sxs-lookup"><span data-stu-id="6439a-112">eas</span></span>|<span data-ttu-id="6439a-113">1</span><span class="sxs-lookup"><span data-stu-id="6439a-113">1</span></span>|<span data-ttu-id="6439a-114">设备管理 Exchange server。</span><span class="sxs-lookup"><span data-stu-id="6439a-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="6439a-115">mdm</span><span class="sxs-lookup"><span data-stu-id="6439a-115">mdm</span></span>|<span data-ttu-id="6439a-116">2</span><span class="sxs-lookup"><span data-stu-id="6439a-116">2</span></span>|<span data-ttu-id="6439a-117">设备管理由 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="6439a-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="6439a-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="6439a-118">easMdm</span></span>|<span data-ttu-id="6439a-119">3</span><span class="sxs-lookup"><span data-stu-id="6439a-119">3</span></span>|<span data-ttu-id="6439a-120">设备所管理的 Exchange server 和 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="6439a-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="6439a-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="6439a-121">intuneClient</span></span>|<span data-ttu-id="6439a-122">4</span><span class="sxs-lookup"><span data-stu-id="6439a-122">4</span></span>|<span data-ttu-id="6439a-123">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="6439a-123">Intune client managed.</span></span>|
|<span data-ttu-id="6439a-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="6439a-124">easIntuneClient</span></span>|<span data-ttu-id="6439a-125">5</span><span class="sxs-lookup"><span data-stu-id="6439a-125">5</span></span>|<span data-ttu-id="6439a-126">设备是 EAS 和 Intune 客户端双托管。</span><span class="sxs-lookup"><span data-stu-id="6439a-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="6439a-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="6439a-127">configurationManagerClient</span></span>|<span data-ttu-id="6439a-128">8</span><span class="sxs-lookup"><span data-stu-id="6439a-128">8</span></span>|<span data-ttu-id="6439a-129">设备管理由配置管理器中。</span><span class="sxs-lookup"><span data-stu-id="6439a-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="6439a-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="6439a-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="6439a-131">10</span><span class="sxs-lookup"><span data-stu-id="6439a-131">10</span></span>|<span data-ttu-id="6439a-132">设备所管理的配置管理器和 mdm。</span><span class="sxs-lookup"><span data-stu-id="6439a-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="6439a-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="6439a-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="6439a-134">11</span><span class="sxs-lookup"><span data-stu-id="6439a-134">11</span></span>|<span data-ttu-id="6439a-135">配置管理器、 MDM 和 Eas 由管理设备。</span><span class="sxs-lookup"><span data-stu-id="6439a-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="6439a-136">unknown</span><span class="sxs-lookup"><span data-stu-id="6439a-136">unknown</span></span>|<span data-ttu-id="6439a-137">16</span><span class="sxs-lookup"><span data-stu-id="6439a-137">16</span></span>|<span data-ttu-id="6439a-138">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="6439a-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="6439a-139">jamf</span><span class="sxs-lookup"><span data-stu-id="6439a-139">jamf</span></span>|<span data-ttu-id="6439a-140">32</span><span class="sxs-lookup"><span data-stu-id="6439a-140">32</span></span>|<span data-ttu-id="6439a-141">从 Jamf 获取设备属性。</span><span class="sxs-lookup"><span data-stu-id="6439a-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="6439a-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="6439a-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="6439a-143">64</span><span class="sxs-lookup"><span data-stu-id="6439a-143">64</span></span>|<span data-ttu-id="6439a-144">由 Google 的 CloudDPC 管理设备。</span><span class="sxs-lookup"><span data-stu-id="6439a-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="6439a-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="6439a-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="6439a-146">258</span><span class="sxs-lookup"><span data-stu-id="6439a-146">258</span></span>|<span data-ttu-id="6439a-147">由 Microsoft 365 通过 Intune 管理此设备。</span><span class="sxs-lookup"><span data-stu-id="6439a-147">This device is managed by Microsoft 365 through Intune.</span></span>|




