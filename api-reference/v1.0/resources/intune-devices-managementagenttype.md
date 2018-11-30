---
title: managementAgentType 枚举类型
description: 管理代理类型。
ms.openlocfilehash: de837f712f69576ea7a862101d2cfaa30b8685d3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010048"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="f270a-103">managementAgentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f270a-103">managementAgentType enum type</span></span>

> <span data-ttu-id="f270a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f270a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f270a-105">管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="f270a-105">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="f270a-106">成员</span><span class="sxs-lookup"><span data-stu-id="f270a-106">Members</span></span>
|<span data-ttu-id="f270a-107">成员</span><span class="sxs-lookup"><span data-stu-id="f270a-107">Member</span></span>|<span data-ttu-id="f270a-108">值</span><span class="sxs-lookup"><span data-stu-id="f270a-108">Value</span></span>|<span data-ttu-id="f270a-109">说明</span><span class="sxs-lookup"><span data-stu-id="f270a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f270a-110">eas</span><span class="sxs-lookup"><span data-stu-id="f270a-110">eas</span></span>|<span data-ttu-id="f270a-111">1</span><span class="sxs-lookup"><span data-stu-id="f270a-111">1</span></span>|<span data-ttu-id="f270a-112">设备管理 Exchange server。</span><span class="sxs-lookup"><span data-stu-id="f270a-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="f270a-113">mdm</span><span class="sxs-lookup"><span data-stu-id="f270a-113">mdm</span></span>|<span data-ttu-id="f270a-114">2</span><span class="sxs-lookup"><span data-stu-id="f270a-114">2</span></span>|<span data-ttu-id="f270a-115">设备管理由 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="f270a-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="f270a-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="f270a-116">easMdm</span></span>|<span data-ttu-id="f270a-117">3</span><span class="sxs-lookup"><span data-stu-id="f270a-117">3</span></span>|<span data-ttu-id="f270a-118">设备所管理的 Exchange server 和 Intune mdm。</span><span class="sxs-lookup"><span data-stu-id="f270a-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="f270a-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="f270a-119">intuneClient</span></span>|<span data-ttu-id="f270a-120">4</span><span class="sxs-lookup"><span data-stu-id="f270a-120">4</span></span>|<span data-ttu-id="f270a-121">Intune 客户端托管。</span><span class="sxs-lookup"><span data-stu-id="f270a-121">Intune client managed.</span></span>|
|<span data-ttu-id="f270a-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="f270a-122">easIntuneClient</span></span>|<span data-ttu-id="f270a-123">5</span><span class="sxs-lookup"><span data-stu-id="f270a-123">5</span></span>|<span data-ttu-id="f270a-124">设备是 EAS 和 Intune 客户端双托管。</span><span class="sxs-lookup"><span data-stu-id="f270a-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="f270a-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="f270a-125">configurationManagerClient</span></span>|<span data-ttu-id="f270a-126">8</span><span class="sxs-lookup"><span data-stu-id="f270a-126">8</span></span>|<span data-ttu-id="f270a-127">设备管理由配置管理器中。</span><span class="sxs-lookup"><span data-stu-id="f270a-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="f270a-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="f270a-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="f270a-129">10</span><span class="sxs-lookup"><span data-stu-id="f270a-129">10</span></span>|<span data-ttu-id="f270a-130">设备所管理的配置管理器和 mdm。</span><span class="sxs-lookup"><span data-stu-id="f270a-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="f270a-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="f270a-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="f270a-132">11</span><span class="sxs-lookup"><span data-stu-id="f270a-132">11</span></span>|<span data-ttu-id="f270a-133">配置管理器、 MDM 和 Eas 由管理设备。</span><span class="sxs-lookup"><span data-stu-id="f270a-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="f270a-134">unknown</span><span class="sxs-lookup"><span data-stu-id="f270a-134">unknown</span></span>|<span data-ttu-id="f270a-135">16</span><span class="sxs-lookup"><span data-stu-id="f270a-135">16</span></span>|<span data-ttu-id="f270a-136">未知的管理代理类型。</span><span class="sxs-lookup"><span data-stu-id="f270a-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="f270a-137">jamf</span><span class="sxs-lookup"><span data-stu-id="f270a-137">jamf</span></span>|<span data-ttu-id="f270a-138">32</span><span class="sxs-lookup"><span data-stu-id="f270a-138">32</span></span>|<span data-ttu-id="f270a-139">从 Jamf 获取设备属性。</span><span class="sxs-lookup"><span data-stu-id="f270a-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="f270a-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="f270a-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="f270a-141">64</span><span class="sxs-lookup"><span data-stu-id="f270a-141">64</span></span>|<span data-ttu-id="f270a-142">由 Google 的 CloudDPC 管理设备。</span><span class="sxs-lookup"><span data-stu-id="f270a-142">The device is managed by Google's CloudDPC.</span></span>|



