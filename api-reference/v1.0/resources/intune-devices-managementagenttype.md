---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d5f698a2878b0662193128044d7b069c8dfe8b3f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406831"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="7ba2a-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7ba2a-103">managementAgentType enum type</span></span>

<span data-ttu-id="7ba2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ba2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ba2a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ba2a-106">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="7ba2a-107">成员</span><span class="sxs-lookup"><span data-stu-id="7ba2a-107">Members</span></span>
|<span data-ttu-id="7ba2a-108">成员</span><span class="sxs-lookup"><span data-stu-id="7ba2a-108">Member</span></span>|<span data-ttu-id="7ba2a-109">值</span><span class="sxs-lookup"><span data-stu-id="7ba2a-109">Value</span></span>|<span data-ttu-id="7ba2a-110">说明</span><span class="sxs-lookup"><span data-stu-id="7ba2a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ba2a-111">符合</span><span class="sxs-lookup"><span data-stu-id="7ba2a-111">eas</span></span>|<span data-ttu-id="7ba2a-112">1</span><span class="sxs-lookup"><span data-stu-id="7ba2a-112">1</span></span>|<span data-ttu-id="7ba2a-113">设备由 Exchange server 管理。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="7ba2a-114">mdm</span><span class="sxs-lookup"><span data-stu-id="7ba2a-114">mdm</span></span>|<span data-ttu-id="7ba2a-115">双面</span><span class="sxs-lookup"><span data-stu-id="7ba2a-115">2</span></span>|<span data-ttu-id="7ba2a-116">设备由 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="7ba2a-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="7ba2a-117">easMdm</span></span>|<span data-ttu-id="7ba2a-118">第三章</span><span class="sxs-lookup"><span data-stu-id="7ba2a-118">3</span></span>|<span data-ttu-id="7ba2a-119">设备由 Exchange server 和 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="7ba2a-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="7ba2a-120">intuneClient</span></span>|<span data-ttu-id="7ba2a-121">4 </span><span class="sxs-lookup"><span data-stu-id="7ba2a-121">4</span></span>|<span data-ttu-id="7ba2a-122">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-122">Intune client managed.</span></span>|
|<span data-ttu-id="7ba2a-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="7ba2a-123">easIntuneClient</span></span>|<span data-ttu-id="7ba2a-124">5 </span><span class="sxs-lookup"><span data-stu-id="7ba2a-124">5</span></span>|<span data-ttu-id="7ba2a-125">设备为 EAS 和 Intune 客户端双重托管。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="7ba2a-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="7ba2a-126">configurationManagerClient</span></span>|<span data-ttu-id="7ba2a-127">8 </span><span class="sxs-lookup"><span data-stu-id="7ba2a-127">8</span></span>|<span data-ttu-id="7ba2a-128">设备由配置管理器管理。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="7ba2a-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="7ba2a-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="7ba2a-130">10 </span><span class="sxs-lookup"><span data-stu-id="7ba2a-130">10</span></span>|<span data-ttu-id="7ba2a-131">设备由 Configuration Manager 和 MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="7ba2a-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="7ba2a-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="7ba2a-133">11x17</span><span class="sxs-lookup"><span data-stu-id="7ba2a-133">11</span></span>|<span data-ttu-id="7ba2a-134">设备由 Configuration Manager、MDM 和 Eas 管理。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="7ba2a-135">unknown</span><span class="sxs-lookup"><span data-stu-id="7ba2a-135">unknown</span></span>|<span data-ttu-id="7ba2a-136">16 </span><span class="sxs-lookup"><span data-stu-id="7ba2a-136">16</span></span>|<span data-ttu-id="7ba2a-137">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="7ba2a-138">jamf</span><span class="sxs-lookup"><span data-stu-id="7ba2a-138">jamf</span></span>|<span data-ttu-id="7ba2a-139">32</span><span class="sxs-lookup"><span data-stu-id="7ba2a-139">32</span></span>|<span data-ttu-id="7ba2a-140">设备属性是从 Jamf 中提取的。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="7ba2a-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="7ba2a-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="7ba2a-142">64</span><span class="sxs-lookup"><span data-stu-id="7ba2a-142">64</span></span>|<span data-ttu-id="7ba2a-143">设备由 Google 的 CloudDPC 管理。</span><span class="sxs-lookup"><span data-stu-id="7ba2a-143">The device is managed by Google's CloudDPC.</span></span>|







