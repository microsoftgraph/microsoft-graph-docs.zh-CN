---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: tfitzmac
ms.openlocfilehash: b1f6db6eaea1a488831bec3d7ff61d6170414956
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355515"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="15183-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="15183-103">managementAgentType enum type</span></span>

> <span data-ttu-id="15183-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="15183-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15183-105">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="15183-105">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="15183-106">成员</span><span class="sxs-lookup"><span data-stu-id="15183-106">Members</span></span>
|<span data-ttu-id="15183-107">成员</span><span class="sxs-lookup"><span data-stu-id="15183-107">Member</span></span>|<span data-ttu-id="15183-108">值</span><span class="sxs-lookup"><span data-stu-id="15183-108">Value</span></span>|<span data-ttu-id="15183-109">说明</span><span class="sxs-lookup"><span data-stu-id="15183-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15183-110">eas</span><span class="sxs-lookup"><span data-stu-id="15183-110">eas</span></span>|<span data-ttu-id="15183-111">1</span><span class="sxs-lookup"><span data-stu-id="15183-111">1</span></span>|<span data-ttu-id="15183-112">设备管理 Exchange server。</span><span class="sxs-lookup"><span data-stu-id="15183-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="15183-113">mdm</span><span class="sxs-lookup"><span data-stu-id="15183-113">mdm</span></span>|<span data-ttu-id="15183-114">2</span><span class="sxs-lookup"><span data-stu-id="15183-114">2</span></span>|<span data-ttu-id="15183-115">设备管理由 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="15183-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="15183-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="15183-116">easMdm</span></span>|<span data-ttu-id="15183-117">3</span><span class="sxs-lookup"><span data-stu-id="15183-117">3</span></span>|<span data-ttu-id="15183-118">设备所管理的 Exchange server 和 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="15183-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="15183-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="15183-119">intuneClient</span></span>|<span data-ttu-id="15183-120">4</span><span class="sxs-lookup"><span data-stu-id="15183-120">4</span></span>|<span data-ttu-id="15183-121">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="15183-121">Intune client managed.</span></span>|
|<span data-ttu-id="15183-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="15183-122">easIntuneClient</span></span>|<span data-ttu-id="15183-123">5</span><span class="sxs-lookup"><span data-stu-id="15183-123">5</span></span>|<span data-ttu-id="15183-124">设备是 EAS 和 Intune 客户端双托管。</span><span class="sxs-lookup"><span data-stu-id="15183-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="15183-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="15183-125">configurationManagerClient</span></span>|<span data-ttu-id="15183-126">8</span><span class="sxs-lookup"><span data-stu-id="15183-126">8</span></span>|<span data-ttu-id="15183-127">设备管理由配置管理器中。</span><span class="sxs-lookup"><span data-stu-id="15183-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="15183-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="15183-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="15183-129">10</span><span class="sxs-lookup"><span data-stu-id="15183-129">10</span></span>|<span data-ttu-id="15183-130">设备所管理的配置管理器和 mdm。</span><span class="sxs-lookup"><span data-stu-id="15183-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="15183-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="15183-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="15183-132">11</span><span class="sxs-lookup"><span data-stu-id="15183-132">11</span></span>|<span data-ttu-id="15183-133">配置管理器、 MDM 和 Eas 由管理设备。</span><span class="sxs-lookup"><span data-stu-id="15183-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="15183-134">unknown</span><span class="sxs-lookup"><span data-stu-id="15183-134">unknown</span></span>|<span data-ttu-id="15183-135">16</span><span class="sxs-lookup"><span data-stu-id="15183-135">16</span></span>|<span data-ttu-id="15183-136">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="15183-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="15183-137">jamf</span><span class="sxs-lookup"><span data-stu-id="15183-137">jamf</span></span>|<span data-ttu-id="15183-138">32</span><span class="sxs-lookup"><span data-stu-id="15183-138">32</span></span>|<span data-ttu-id="15183-139">从 Jamf 获取设备属性。</span><span class="sxs-lookup"><span data-stu-id="15183-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="15183-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="15183-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="15183-141">64</span><span class="sxs-lookup"><span data-stu-id="15183-141">64</span></span>|<span data-ttu-id="15183-142">由 Google 的 CloudDPC 管理设备。</span><span class="sxs-lookup"><span data-stu-id="15183-142">The device is managed by Google's CloudDPC.</span></span>|



