---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0a11300891ca4b12b15de26b5be929823b4a8ddf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751354"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="2dae7-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2dae7-103">managementAgentType enum type</span></span>

<span data-ttu-id="2dae7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dae7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2dae7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2dae7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dae7-106">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="2dae7-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="2dae7-107">成员</span><span class="sxs-lookup"><span data-stu-id="2dae7-107">Members</span></span>
|<span data-ttu-id="2dae7-108">成员</span><span class="sxs-lookup"><span data-stu-id="2dae7-108">Member</span></span>|<span data-ttu-id="2dae7-109">值</span><span class="sxs-lookup"><span data-stu-id="2dae7-109">Value</span></span>|<span data-ttu-id="2dae7-110">说明</span><span class="sxs-lookup"><span data-stu-id="2dae7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dae7-111">eas</span><span class="sxs-lookup"><span data-stu-id="2dae7-111">eas</span></span>|<span data-ttu-id="2dae7-112">1</span><span class="sxs-lookup"><span data-stu-id="2dae7-112">1</span></span>|<span data-ttu-id="2dae7-113">设备由Exchange管理。</span><span class="sxs-lookup"><span data-stu-id="2dae7-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="2dae7-114">mdm</span><span class="sxs-lookup"><span data-stu-id="2dae7-114">mdm</span></span>|<span data-ttu-id="2dae7-115">2</span><span class="sxs-lookup"><span data-stu-id="2dae7-115">2</span></span>|<span data-ttu-id="2dae7-116">设备由 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="2dae7-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="2dae7-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="2dae7-117">easMdm</span></span>|<span data-ttu-id="2dae7-118">3</span><span class="sxs-lookup"><span data-stu-id="2dae7-118">3</span></span>|<span data-ttu-id="2dae7-119">设备由托管服务器Exchange Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="2dae7-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="2dae7-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="2dae7-120">intuneClient</span></span>|<span data-ttu-id="2dae7-121">4 </span><span class="sxs-lookup"><span data-stu-id="2dae7-121">4</span></span>|<span data-ttu-id="2dae7-122">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="2dae7-122">Intune client managed.</span></span>|
|<span data-ttu-id="2dae7-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="2dae7-123">easIntuneClient</span></span>|<span data-ttu-id="2dae7-124">5 </span><span class="sxs-lookup"><span data-stu-id="2dae7-124">5</span></span>|<span data-ttu-id="2dae7-125">设备是 EAS 和 Intune 客户端双托管设备。</span><span class="sxs-lookup"><span data-stu-id="2dae7-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="2dae7-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="2dae7-126">configurationManagerClient</span></span>|<span data-ttu-id="2dae7-127">8 </span><span class="sxs-lookup"><span data-stu-id="2dae7-127">8</span></span>|<span data-ttu-id="2dae7-128">设备由 Configuration Manager 管理。</span><span class="sxs-lookup"><span data-stu-id="2dae7-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="2dae7-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="2dae7-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="2dae7-130">10  </span><span class="sxs-lookup"><span data-stu-id="2dae7-130">10</span></span>|<span data-ttu-id="2dae7-131">设备由 Configuration Manager 和 MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="2dae7-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="2dae7-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="2dae7-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="2dae7-133">11</span><span class="sxs-lookup"><span data-stu-id="2dae7-133">11</span></span>|<span data-ttu-id="2dae7-134">设备由 Configuration Manager、MDM 和 Eas 管理。</span><span class="sxs-lookup"><span data-stu-id="2dae7-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="2dae7-135">unknown</span><span class="sxs-lookup"><span data-stu-id="2dae7-135">unknown</span></span>|<span data-ttu-id="2dae7-136">16 </span><span class="sxs-lookup"><span data-stu-id="2dae7-136">16</span></span>|<span data-ttu-id="2dae7-137">未知管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="2dae7-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="2dae7-138">jamf</span><span class="sxs-lookup"><span data-stu-id="2dae7-138">jamf</span></span>|<span data-ttu-id="2dae7-139">32</span><span class="sxs-lookup"><span data-stu-id="2dae7-139">32</span></span>|<span data-ttu-id="2dae7-140">设备属性从 Jamf 获取。</span><span class="sxs-lookup"><span data-stu-id="2dae7-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="2dae7-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="2dae7-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="2dae7-142">64</span><span class="sxs-lookup"><span data-stu-id="2dae7-142">64</span></span>|<span data-ttu-id="2dae7-143">设备由 Google 的 CloudDPC 管理。</span><span class="sxs-lookup"><span data-stu-id="2dae7-143">The device is managed by Google's CloudDPC.</span></span>|




