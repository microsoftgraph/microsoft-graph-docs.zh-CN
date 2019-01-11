---
title: embeddedSIMDeviceStateValue 枚举类型
description: 介绍为嵌入 SIM 激活代码的各种状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a3974c0df65ef9f59242f390b7166e11c3e0c592
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886056"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="e10d6-103">embeddedSIMDeviceStateValue 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e10d6-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="e10d6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e10d6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e10d6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e10d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e10d6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e10d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e10d6-107">介绍为嵌入 SIM 激活代码的各种状态。</span><span class="sxs-lookup"><span data-stu-id="e10d6-107">Describes the various states for an embedded SIM activation code.</span></span>
## <a name="members"></a><span data-ttu-id="e10d6-108">成员</span><span class="sxs-lookup"><span data-stu-id="e10d6-108">Members</span></span>
|<span data-ttu-id="e10d6-109">成员</span><span class="sxs-lookup"><span data-stu-id="e10d6-109">Member</span></span>|<span data-ttu-id="e10d6-110">值</span><span class="sxs-lookup"><span data-stu-id="e10d6-110">Value</span></span>|<span data-ttu-id="e10d6-111">Description</span><span class="sxs-lookup"><span data-stu-id="e10d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e10d6-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="e10d6-112">notEvaluated</span></span>|<span data-ttu-id="e10d6-113">0</span><span class="sxs-lookup"><span data-stu-id="e10d6-113">0</span></span>|<span data-ttu-id="e10d6-114">指定嵌入的 SIM 激活代码可用，并且可以分配给设备。</span><span class="sxs-lookup"><span data-stu-id="e10d6-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="e10d6-115">failed</span><span class="sxs-lookup"><span data-stu-id="e10d6-115">failed</span></span>|<span data-ttu-id="e10d6-116">1</span><span class="sxs-lookup"><span data-stu-id="e10d6-116">1</span></span>|<span data-ttu-id="e10d6-117">指定 Intune 服务未能向设备提供此配置文件。</span><span class="sxs-lookup"><span data-stu-id="e10d6-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="e10d6-118">安装</span><span class="sxs-lookup"><span data-stu-id="e10d6-118">installing</span></span>|<span data-ttu-id="e10d6-119">2</span><span class="sxs-lookup"><span data-stu-id="e10d6-119">2</span></span>|<span data-ttu-id="e10d6-120">指定的嵌入式的 SIM 激活代码已分配给设备和设备安装令牌。</span><span class="sxs-lookup"><span data-stu-id="e10d6-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="e10d6-121">安装</span><span class="sxs-lookup"><span data-stu-id="e10d6-121">installed</span></span>|<span data-ttu-id="e10d6-122">3</span><span class="sxs-lookup"><span data-stu-id="e10d6-122">3</span></span>|<span data-ttu-id="e10d6-123">指定已成功目标设备上安装的嵌入的 SIM 激活代码。</span><span class="sxs-lookup"><span data-stu-id="e10d6-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="e10d6-124">删除</span><span class="sxs-lookup"><span data-stu-id="e10d6-124">deleting</span></span>|<span data-ttu-id="e10d6-125">4</span><span class="sxs-lookup"><span data-stu-id="e10d6-125">4</span></span>|<span data-ttu-id="e10d6-126">指定 Intune 服务尝试从设备中删除配置文件。</span><span class="sxs-lookup"><span data-stu-id="e10d6-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="e10d6-127">error</span><span class="sxs-lookup"><span data-stu-id="e10d6-127">error</span></span>|<span data-ttu-id="e10d6-128">5</span><span class="sxs-lookup"><span data-stu-id="e10d6-128">5</span></span>|<span data-ttu-id="e10d6-129">指定存在与此配置文件的错误。</span><span class="sxs-lookup"><span data-stu-id="e10d6-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="e10d6-130">deleted</span><span class="sxs-lookup"><span data-stu-id="e10d6-130">deleted</span></span>|<span data-ttu-id="e10d6-131">6</span><span class="sxs-lookup"><span data-stu-id="e10d6-131">6</span></span>|<span data-ttu-id="e10d6-132">指定从设备中删除配置文件。</span><span class="sxs-lookup"><span data-stu-id="e10d6-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="e10d6-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="e10d6-133">removedByUser</span></span>|<span data-ttu-id="e10d6-134">7</span><span class="sxs-lookup"><span data-stu-id="e10d6-134">7</span></span>|<span data-ttu-id="e10d6-135">指定从设备删除配置文件的用户</span><span class="sxs-lookup"><span data-stu-id="e10d6-135">Designates that the profile is removed from the device by the user</span></span>|





