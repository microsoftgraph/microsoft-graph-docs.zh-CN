---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a5835a0a8ca83cef2d5590679ce8aa4e77b0859
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530294"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="63b38-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="63b38-103">managementAgentType enum type</span></span>

<span data-ttu-id="63b38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63b38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63b38-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63b38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63b38-106">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="63b38-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="63b38-107">成员</span><span class="sxs-lookup"><span data-stu-id="63b38-107">Members</span></span>
|<span data-ttu-id="63b38-108">成员</span><span class="sxs-lookup"><span data-stu-id="63b38-108">Member</span></span>|<span data-ttu-id="63b38-109">值</span><span class="sxs-lookup"><span data-stu-id="63b38-109">Value</span></span>|<span data-ttu-id="63b38-110">说明</span><span class="sxs-lookup"><span data-stu-id="63b38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63b38-111">符合</span><span class="sxs-lookup"><span data-stu-id="63b38-111">eas</span></span>|<span data-ttu-id="63b38-112">1 </span><span class="sxs-lookup"><span data-stu-id="63b38-112">1</span></span>|<span data-ttu-id="63b38-113">设备由 Exchange server 管理。</span><span class="sxs-lookup"><span data-stu-id="63b38-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="63b38-114">mdm</span><span class="sxs-lookup"><span data-stu-id="63b38-114">mdm</span></span>|<span data-ttu-id="63b38-115">2 </span><span class="sxs-lookup"><span data-stu-id="63b38-115">2</span></span>|<span data-ttu-id="63b38-116">设备由 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="63b38-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="63b38-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="63b38-117">easMdm</span></span>|<span data-ttu-id="63b38-118">3 </span><span class="sxs-lookup"><span data-stu-id="63b38-118">3</span></span>|<span data-ttu-id="63b38-119">设备由 Exchange server 和 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="63b38-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="63b38-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="63b38-120">intuneClient</span></span>|<span data-ttu-id="63b38-121">4 </span><span class="sxs-lookup"><span data-stu-id="63b38-121">4</span></span>|<span data-ttu-id="63b38-122">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="63b38-122">Intune client managed.</span></span>|
|<span data-ttu-id="63b38-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="63b38-123">easIntuneClient</span></span>|<span data-ttu-id="63b38-124">5 </span><span class="sxs-lookup"><span data-stu-id="63b38-124">5</span></span>|<span data-ttu-id="63b38-125">设备为 EAS 和 Intune 客户端双重托管。</span><span class="sxs-lookup"><span data-stu-id="63b38-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="63b38-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="63b38-126">configurationManagerClient</span></span>|<span data-ttu-id="63b38-127">8 </span><span class="sxs-lookup"><span data-stu-id="63b38-127">8</span></span>|<span data-ttu-id="63b38-128">设备由配置管理器管理。</span><span class="sxs-lookup"><span data-stu-id="63b38-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="63b38-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="63b38-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="63b38-130">10 </span><span class="sxs-lookup"><span data-stu-id="63b38-130">10</span></span>|<span data-ttu-id="63b38-131">设备由 Configuration Manager 和 MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="63b38-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="63b38-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="63b38-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="63b38-133">11x17</span><span class="sxs-lookup"><span data-stu-id="63b38-133">11</span></span>|<span data-ttu-id="63b38-134">设备由 Configuration Manager、MDM 和 Eas 管理。</span><span class="sxs-lookup"><span data-stu-id="63b38-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="63b38-135">unknown</span><span class="sxs-lookup"><span data-stu-id="63b38-135">unknown</span></span>|<span data-ttu-id="63b38-136">16 </span><span class="sxs-lookup"><span data-stu-id="63b38-136">16</span></span>|<span data-ttu-id="63b38-137">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="63b38-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="63b38-138">jamf</span><span class="sxs-lookup"><span data-stu-id="63b38-138">jamf</span></span>|<span data-ttu-id="63b38-139">32</span><span class="sxs-lookup"><span data-stu-id="63b38-139">32</span></span>|<span data-ttu-id="63b38-140">设备属性是从 Jamf 中提取的。</span><span class="sxs-lookup"><span data-stu-id="63b38-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="63b38-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="63b38-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="63b38-142">64</span><span class="sxs-lookup"><span data-stu-id="63b38-142">64</span></span>|<span data-ttu-id="63b38-143">设备由 Google 的 CloudDPC 管理。</span><span class="sxs-lookup"><span data-stu-id="63b38-143">The device is managed by Google's CloudDPC.</span></span>|




