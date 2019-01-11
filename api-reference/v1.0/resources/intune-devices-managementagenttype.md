---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 66441a37b417cef13cbb09219a26a98250cbf610
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888485"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="b8b5c-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b8b5c-103">managementAgentType enum type</span></span>

> <span data-ttu-id="b8b5c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8b5c-105">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-105">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="b8b5c-106">成员</span><span class="sxs-lookup"><span data-stu-id="b8b5c-106">Members</span></span>
|<span data-ttu-id="b8b5c-107">成员</span><span class="sxs-lookup"><span data-stu-id="b8b5c-107">Member</span></span>|<span data-ttu-id="b8b5c-108">值</span><span class="sxs-lookup"><span data-stu-id="b8b5c-108">Value</span></span>|<span data-ttu-id="b8b5c-109">Description</span><span class="sxs-lookup"><span data-stu-id="b8b5c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8b5c-110">eas</span><span class="sxs-lookup"><span data-stu-id="b8b5c-110">eas</span></span>|<span data-ttu-id="b8b5c-111">1</span><span class="sxs-lookup"><span data-stu-id="b8b5c-111">1</span></span>|<span data-ttu-id="b8b5c-112">设备管理 Exchange server。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="b8b5c-113">mdm</span><span class="sxs-lookup"><span data-stu-id="b8b5c-113">mdm</span></span>|<span data-ttu-id="b8b5c-114">2</span><span class="sxs-lookup"><span data-stu-id="b8b5c-114">2</span></span>|<span data-ttu-id="b8b5c-115">设备管理由 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="b8b5c-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="b8b5c-116">easMdm</span></span>|<span data-ttu-id="b8b5c-117">3</span><span class="sxs-lookup"><span data-stu-id="b8b5c-117">3</span></span>|<span data-ttu-id="b8b5c-118">设备所管理的 Exchange server 和 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="b8b5c-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="b8b5c-119">intuneClient</span></span>|<span data-ttu-id="b8b5c-120">4</span><span class="sxs-lookup"><span data-stu-id="b8b5c-120">4</span></span>|<span data-ttu-id="b8b5c-121">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-121">Intune client managed.</span></span>|
|<span data-ttu-id="b8b5c-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="b8b5c-122">easIntuneClient</span></span>|<span data-ttu-id="b8b5c-123">5</span><span class="sxs-lookup"><span data-stu-id="b8b5c-123">5</span></span>|<span data-ttu-id="b8b5c-124">设备是 EAS 和 Intune 客户端双托管。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="b8b5c-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="b8b5c-125">configurationManagerClient</span></span>|<span data-ttu-id="b8b5c-126">8</span><span class="sxs-lookup"><span data-stu-id="b8b5c-126">8</span></span>|<span data-ttu-id="b8b5c-127">设备管理由配置管理器中。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="b8b5c-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="b8b5c-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="b8b5c-129">10</span><span class="sxs-lookup"><span data-stu-id="b8b5c-129">10</span></span>|<span data-ttu-id="b8b5c-130">设备所管理的配置管理器和 mdm。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="b8b5c-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="b8b5c-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="b8b5c-132">11</span><span class="sxs-lookup"><span data-stu-id="b8b5c-132">11</span></span>|<span data-ttu-id="b8b5c-133">配置管理器、 MDM 和 Eas 由管理设备。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="b8b5c-134">unknown</span><span class="sxs-lookup"><span data-stu-id="b8b5c-134">unknown</span></span>|<span data-ttu-id="b8b5c-135">16</span><span class="sxs-lookup"><span data-stu-id="b8b5c-135">16</span></span>|<span data-ttu-id="b8b5c-136">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="b8b5c-137">jamf</span><span class="sxs-lookup"><span data-stu-id="b8b5c-137">jamf</span></span>|<span data-ttu-id="b8b5c-138">32</span><span class="sxs-lookup"><span data-stu-id="b8b5c-138">32</span></span>|<span data-ttu-id="b8b5c-139">从 Jamf 获取设备属性。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="b8b5c-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="b8b5c-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="b8b5c-141">64</span><span class="sxs-lookup"><span data-stu-id="b8b5c-141">64</span></span>|<span data-ttu-id="b8b5c-142">由 Google 的 CloudDPC 管理设备。</span><span class="sxs-lookup"><span data-stu-id="b8b5c-142">The device is managed by Google's CloudDPC.</span></span>|



