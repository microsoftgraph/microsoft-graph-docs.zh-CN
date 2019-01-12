---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b76231a2781a153c5384c1dc3efdf8facec04dcc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966165"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="9c2e9-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9c2e9-103">managementAgentType enum type</span></span>

> <span data-ttu-id="9c2e9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c2e9-105">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-105">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="9c2e9-106">成员</span><span class="sxs-lookup"><span data-stu-id="9c2e9-106">Members</span></span>
|<span data-ttu-id="9c2e9-107">成员</span><span class="sxs-lookup"><span data-stu-id="9c2e9-107">Member</span></span>|<span data-ttu-id="9c2e9-108">值</span><span class="sxs-lookup"><span data-stu-id="9c2e9-108">Value</span></span>|<span data-ttu-id="9c2e9-109">Description</span><span class="sxs-lookup"><span data-stu-id="9c2e9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c2e9-110">eas</span><span class="sxs-lookup"><span data-stu-id="9c2e9-110">eas</span></span>|<span data-ttu-id="9c2e9-111">1</span><span class="sxs-lookup"><span data-stu-id="9c2e9-111">1</span></span>|<span data-ttu-id="9c2e9-112">设备管理 Exchange server。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="9c2e9-113">mdm</span><span class="sxs-lookup"><span data-stu-id="9c2e9-113">mdm</span></span>|<span data-ttu-id="9c2e9-114">2</span><span class="sxs-lookup"><span data-stu-id="9c2e9-114">2</span></span>|<span data-ttu-id="9c2e9-115">设备管理由 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="9c2e9-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="9c2e9-116">easMdm</span></span>|<span data-ttu-id="9c2e9-117">3</span><span class="sxs-lookup"><span data-stu-id="9c2e9-117">3</span></span>|<span data-ttu-id="9c2e9-118">设备所管理的 Exchange server 和 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="9c2e9-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="9c2e9-119">intuneClient</span></span>|<span data-ttu-id="9c2e9-120">4</span><span class="sxs-lookup"><span data-stu-id="9c2e9-120">4</span></span>|<span data-ttu-id="9c2e9-121">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-121">Intune client managed.</span></span>|
|<span data-ttu-id="9c2e9-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="9c2e9-122">easIntuneClient</span></span>|<span data-ttu-id="9c2e9-123">5</span><span class="sxs-lookup"><span data-stu-id="9c2e9-123">5</span></span>|<span data-ttu-id="9c2e9-124">设备是 EAS 和 Intune 客户端双托管。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="9c2e9-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="9c2e9-125">configurationManagerClient</span></span>|<span data-ttu-id="9c2e9-126">8</span><span class="sxs-lookup"><span data-stu-id="9c2e9-126">8</span></span>|<span data-ttu-id="9c2e9-127">设备管理由配置管理器中。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="9c2e9-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="9c2e9-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="9c2e9-129">10</span><span class="sxs-lookup"><span data-stu-id="9c2e9-129">10</span></span>|<span data-ttu-id="9c2e9-130">设备所管理的配置管理器和 mdm。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="9c2e9-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="9c2e9-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="9c2e9-132">11</span><span class="sxs-lookup"><span data-stu-id="9c2e9-132">11</span></span>|<span data-ttu-id="9c2e9-133">配置管理器、 MDM 和 Eas 由管理设备。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="9c2e9-134">unknown</span><span class="sxs-lookup"><span data-stu-id="9c2e9-134">unknown</span></span>|<span data-ttu-id="9c2e9-135">16</span><span class="sxs-lookup"><span data-stu-id="9c2e9-135">16</span></span>|<span data-ttu-id="9c2e9-136">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="9c2e9-137">jamf</span><span class="sxs-lookup"><span data-stu-id="9c2e9-137">jamf</span></span>|<span data-ttu-id="9c2e9-138">32</span><span class="sxs-lookup"><span data-stu-id="9c2e9-138">32</span></span>|<span data-ttu-id="9c2e9-139">从 Jamf 获取设备属性。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="9c2e9-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="9c2e9-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="9c2e9-141">64</span><span class="sxs-lookup"><span data-stu-id="9c2e9-141">64</span></span>|<span data-ttu-id="9c2e9-142">由 Google 的 CloudDPC 管理设备。</span><span class="sxs-lookup"><span data-stu-id="9c2e9-142">The device is managed by Google's CloudDPC.</span></span>|



