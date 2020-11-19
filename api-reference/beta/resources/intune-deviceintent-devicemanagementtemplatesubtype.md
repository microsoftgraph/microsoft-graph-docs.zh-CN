---
title: deviceManagementTemplateSubtype 枚举类型
description: Template 子类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6766834a860d06501cd34a423c457f5ac584b6d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209442"
---
# <a name="devicemanagementtemplatesubtype-enum-type"></a><span data-ttu-id="847a7-103">deviceManagementTemplateSubtype 枚举类型</span><span class="sxs-lookup"><span data-stu-id="847a7-103">deviceManagementTemplateSubtype enum type</span></span>

<span data-ttu-id="847a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="847a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="847a7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="847a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="847a7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="847a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="847a7-107">Template 子类型</span><span class="sxs-lookup"><span data-stu-id="847a7-107">Template subtype</span></span>

## <a name="members"></a><span data-ttu-id="847a7-108">成员</span><span class="sxs-lookup"><span data-stu-id="847a7-108">Members</span></span>
|<span data-ttu-id="847a7-109">成员</span><span class="sxs-lookup"><span data-stu-id="847a7-109">Member</span></span>|<span data-ttu-id="847a7-110">值</span><span class="sxs-lookup"><span data-stu-id="847a7-110">Value</span></span>|<span data-ttu-id="847a7-111">说明</span><span class="sxs-lookup"><span data-stu-id="847a7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="847a7-112">无</span><span class="sxs-lookup"><span data-stu-id="847a7-112">none</span></span>|<span data-ttu-id="847a7-113">0</span><span class="sxs-lookup"><span data-stu-id="847a7-113">0</span></span>|<span data-ttu-id="847a7-114">模板没有子类型</span><span class="sxs-lookup"><span data-stu-id="847a7-114">Template has no subtype</span></span>|
|<span data-ttu-id="847a7-115">firewall</span><span class="sxs-lookup"><span data-stu-id="847a7-115">firewall</span></span>|<span data-ttu-id="847a7-116">1</span><span class="sxs-lookup"><span data-stu-id="847a7-116">1</span></span>|<span data-ttu-id="847a7-117">终结点安全防火墙子类型</span><span class="sxs-lookup"><span data-stu-id="847a7-117">Endpoint security firewall subtype</span></span>|
|<span data-ttu-id="847a7-118">diskEncryption</span><span class="sxs-lookup"><span data-stu-id="847a7-118">diskEncryption</span></span>|<span data-ttu-id="847a7-119">双面</span><span class="sxs-lookup"><span data-stu-id="847a7-119">2</span></span>|<span data-ttu-id="847a7-120">终结点安全磁盘加密子类型</span><span class="sxs-lookup"><span data-stu-id="847a7-120">Endpoint security disk encryption subtype</span></span>|
|<span data-ttu-id="847a7-121">attackSurfaceReduction</span><span class="sxs-lookup"><span data-stu-id="847a7-121">attackSurfaceReduction</span></span>|<span data-ttu-id="847a7-122">第三章</span><span class="sxs-lookup"><span data-stu-id="847a7-122">3</span></span>|<span data-ttu-id="847a7-123">终结点安全攻击面缩减子类型</span><span class="sxs-lookup"><span data-stu-id="847a7-123">Endpoint security attack surface reduction subtype</span></span>|
|<span data-ttu-id="847a7-124">endpointDetectionReponse</span><span class="sxs-lookup"><span data-stu-id="847a7-124">endpointDetectionReponse</span></span>|<span data-ttu-id="847a7-125">4 </span><span class="sxs-lookup"><span data-stu-id="847a7-125">4</span></span>|<span data-ttu-id="847a7-126">终结点安全终结点检测和响应子类型</span><span class="sxs-lookup"><span data-stu-id="847a7-126">Endpoint security endpoint detection and response subtype</span></span>|
|<span data-ttu-id="847a7-127">accountProtection</span><span class="sxs-lookup"><span data-stu-id="847a7-127">accountProtection</span></span>|<span data-ttu-id="847a7-128">5 </span><span class="sxs-lookup"><span data-stu-id="847a7-128">5</span></span>|<span data-ttu-id="847a7-129">Endpoint security 帐户保护子类型</span><span class="sxs-lookup"><span data-stu-id="847a7-129">Endpoint security account protection subtype</span></span>|
|<span data-ttu-id="847a7-130">程序</span><span class="sxs-lookup"><span data-stu-id="847a7-130">antivirus</span></span>|<span data-ttu-id="847a7-131">6 </span><span class="sxs-lookup"><span data-stu-id="847a7-131">6</span></span>|<span data-ttu-id="847a7-132">Endpoint security anitivirus 子类型</span><span class="sxs-lookup"><span data-stu-id="847a7-132">Endpoint security anitivirus subtype</span></span>|
|<span data-ttu-id="847a7-133">firewallSharedAppList</span><span class="sxs-lookup"><span data-stu-id="847a7-133">firewallSharedAppList</span></span>|<span data-ttu-id="847a7-134">7 </span><span class="sxs-lookup"><span data-stu-id="847a7-134">7</span></span>|<span data-ttu-id="847a7-135">终结点安全防火墙共享应用程序子类型</span><span class="sxs-lookup"><span data-stu-id="847a7-135">Endpoint security firewall shared app subtype</span></span>|
|<span data-ttu-id="847a7-136">firewallSharedIpList</span><span class="sxs-lookup"><span data-stu-id="847a7-136">firewallSharedIpList</span></span>|<span data-ttu-id="847a7-137">8 </span><span class="sxs-lookup"><span data-stu-id="847a7-137">8</span></span>|<span data-ttu-id="847a7-138">终结点安全防火墙共享 ip 范围列表子类型</span><span class="sxs-lookup"><span data-stu-id="847a7-138">Endpoint security firewall shared ip range list subtype</span></span>|
|<span data-ttu-id="847a7-139">firewallSharedPortlist</span><span class="sxs-lookup"><span data-stu-id="847a7-139">firewallSharedPortlist</span></span>|<span data-ttu-id="847a7-140">9 </span><span class="sxs-lookup"><span data-stu-id="847a7-140">9</span></span>|<span data-ttu-id="847a7-141">终结点安全防火墙共享端口范围列表子类型</span><span class="sxs-lookup"><span data-stu-id="847a7-141">Endpoint security firewall shared port range list subtype</span></span>|




