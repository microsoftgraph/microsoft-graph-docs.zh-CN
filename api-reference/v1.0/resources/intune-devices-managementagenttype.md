---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251564"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="612a3-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="612a3-103">managementAgentType enum type</span></span>

> <span data-ttu-id="612a3-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="612a3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="612a3-105">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="612a3-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="612a3-106">成员</span><span class="sxs-lookup"><span data-stu-id="612a3-106">Members</span></span>
|<span data-ttu-id="612a3-107">成员</span><span class="sxs-lookup"><span data-stu-id="612a3-107">Member</span></span>|<span data-ttu-id="612a3-108">值</span><span class="sxs-lookup"><span data-stu-id="612a3-108">Value</span></span>|<span data-ttu-id="612a3-109">说明</span><span class="sxs-lookup"><span data-stu-id="612a3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="612a3-110">符合</span><span class="sxs-lookup"><span data-stu-id="612a3-110">eas</span></span>|<span data-ttu-id="612a3-111">1</span><span class="sxs-lookup"><span data-stu-id="612a3-111">1</span></span>|<span data-ttu-id="612a3-112">设备由 Exchange server 管理。</span><span class="sxs-lookup"><span data-stu-id="612a3-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="612a3-113">mdm</span><span class="sxs-lookup"><span data-stu-id="612a3-113">mdm</span></span>|<span data-ttu-id="612a3-114">双面</span><span class="sxs-lookup"><span data-stu-id="612a3-114">2</span></span>|<span data-ttu-id="612a3-115">设备由 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="612a3-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="612a3-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="612a3-116">easMdm</span></span>|<span data-ttu-id="612a3-117">第三章</span><span class="sxs-lookup"><span data-stu-id="612a3-117">3</span></span>|<span data-ttu-id="612a3-118">设备由 Exchange server 和 Intune MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="612a3-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="612a3-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="612a3-119">intuneClient</span></span>|<span data-ttu-id="612a3-120">4</span><span class="sxs-lookup"><span data-stu-id="612a3-120">4</span></span>|<span data-ttu-id="612a3-121">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="612a3-121">Intune client managed.</span></span>|
|<span data-ttu-id="612a3-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="612a3-122">easIntuneClient</span></span>|<span data-ttu-id="612a3-123">5</span><span class="sxs-lookup"><span data-stu-id="612a3-123">5</span></span>|<span data-ttu-id="612a3-124">设备为 EAS 和 Intune 客户端双重托管。</span><span class="sxs-lookup"><span data-stu-id="612a3-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="612a3-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="612a3-125">configurationManagerClient</span></span>|<span data-ttu-id="612a3-126">utf-8</span><span class="sxs-lookup"><span data-stu-id="612a3-126">8</span></span>|<span data-ttu-id="612a3-127">设备由配置管理器管理。</span><span class="sxs-lookup"><span data-stu-id="612a3-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="612a3-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="612a3-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="612a3-129">10</span><span class="sxs-lookup"><span data-stu-id="612a3-129">10</span></span>|<span data-ttu-id="612a3-130">设备由 Configuration Manager 和 MDM 管理。</span><span class="sxs-lookup"><span data-stu-id="612a3-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="612a3-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="612a3-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="612a3-132">11x17</span><span class="sxs-lookup"><span data-stu-id="612a3-132">11</span></span>|<span data-ttu-id="612a3-133">设备由 Configuration Manager、MDM 和 Eas 管理。</span><span class="sxs-lookup"><span data-stu-id="612a3-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="612a3-134">unknown</span><span class="sxs-lookup"><span data-stu-id="612a3-134">unknown</span></span>|<span data-ttu-id="612a3-135">位</span><span class="sxs-lookup"><span data-stu-id="612a3-135">16</span></span>|<span data-ttu-id="612a3-136">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="612a3-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="612a3-137">jamf</span><span class="sxs-lookup"><span data-stu-id="612a3-137">jamf</span></span>|<span data-ttu-id="612a3-138">32</span><span class="sxs-lookup"><span data-stu-id="612a3-138">32</span></span>|<span data-ttu-id="612a3-139">设备属性是从 Jamf 中提取的。</span><span class="sxs-lookup"><span data-stu-id="612a3-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="612a3-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="612a3-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="612a3-141">64</span><span class="sxs-lookup"><span data-stu-id="612a3-141">64</span></span>|<span data-ttu-id="612a3-142">设备由 Google 的 CloudDPC 管理。</span><span class="sxs-lookup"><span data-stu-id="612a3-142">The device is managed by Google's CloudDPC.</span></span>|



