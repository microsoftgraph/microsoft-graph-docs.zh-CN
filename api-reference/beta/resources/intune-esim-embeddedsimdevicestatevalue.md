---
title: embeddedSIMDeviceStateValue 枚举类型
description: 介绍为嵌入 SIM 激活代码的各种状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2da255ef2d0cf192dd09a6351bbd337f3cd9b5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421324"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="67f4c-103">embeddedSIMDeviceStateValue 枚举类型</span><span class="sxs-lookup"><span data-stu-id="67f4c-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="67f4c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="67f4c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="67f4c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="67f4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67f4c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67f4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67f4c-107">介绍为嵌入 SIM 激活代码的各种状态。</span><span class="sxs-lookup"><span data-stu-id="67f4c-107">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="67f4c-108">成员</span><span class="sxs-lookup"><span data-stu-id="67f4c-108">Members</span></span>
|<span data-ttu-id="67f4c-109">成员</span><span class="sxs-lookup"><span data-stu-id="67f4c-109">Member</span></span>|<span data-ttu-id="67f4c-110">值</span><span class="sxs-lookup"><span data-stu-id="67f4c-110">Value</span></span>|<span data-ttu-id="67f4c-111">说明</span><span class="sxs-lookup"><span data-stu-id="67f4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67f4c-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="67f4c-112">notEvaluated</span></span>|<span data-ttu-id="67f4c-113">0</span><span class="sxs-lookup"><span data-stu-id="67f4c-113">0</span></span>|<span data-ttu-id="67f4c-114">指定嵌入的 SIM 激活代码可用，并且可以分配给设备。</span><span class="sxs-lookup"><span data-stu-id="67f4c-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="67f4c-115">failed</span><span class="sxs-lookup"><span data-stu-id="67f4c-115">failed</span></span>|<span data-ttu-id="67f4c-116">1</span><span class="sxs-lookup"><span data-stu-id="67f4c-116">1</span></span>|<span data-ttu-id="67f4c-117">指定 Intune 服务未能向设备提供此配置文件。</span><span class="sxs-lookup"><span data-stu-id="67f4c-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="67f4c-118">安装</span><span class="sxs-lookup"><span data-stu-id="67f4c-118">installing</span></span>|<span data-ttu-id="67f4c-119">2</span><span class="sxs-lookup"><span data-stu-id="67f4c-119">2</span></span>|<span data-ttu-id="67f4c-120">指定的嵌入式的 SIM 激活代码已分配给设备和设备安装令牌。</span><span class="sxs-lookup"><span data-stu-id="67f4c-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="67f4c-121">安装</span><span class="sxs-lookup"><span data-stu-id="67f4c-121">installed</span></span>|<span data-ttu-id="67f4c-122">3</span><span class="sxs-lookup"><span data-stu-id="67f4c-122">3</span></span>|<span data-ttu-id="67f4c-123">指定已成功目标设备上安装的嵌入的 SIM 激活代码。</span><span class="sxs-lookup"><span data-stu-id="67f4c-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="67f4c-124">删除</span><span class="sxs-lookup"><span data-stu-id="67f4c-124">deleting</span></span>|<span data-ttu-id="67f4c-125">4</span><span class="sxs-lookup"><span data-stu-id="67f4c-125">4</span></span>|<span data-ttu-id="67f4c-126">指定 Intune 服务尝试从设备中删除配置文件。</span><span class="sxs-lookup"><span data-stu-id="67f4c-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="67f4c-127">error</span><span class="sxs-lookup"><span data-stu-id="67f4c-127">error</span></span>|<span data-ttu-id="67f4c-128">5</span><span class="sxs-lookup"><span data-stu-id="67f4c-128">5</span></span>|<span data-ttu-id="67f4c-129">指定存在与此配置文件的错误。</span><span class="sxs-lookup"><span data-stu-id="67f4c-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="67f4c-130">deleted</span><span class="sxs-lookup"><span data-stu-id="67f4c-130">deleted</span></span>|<span data-ttu-id="67f4c-131">6</span><span class="sxs-lookup"><span data-stu-id="67f4c-131">6</span></span>|<span data-ttu-id="67f4c-132">指定从设备中删除配置文件。</span><span class="sxs-lookup"><span data-stu-id="67f4c-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="67f4c-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="67f4c-133">removedByUser</span></span>|<span data-ttu-id="67f4c-134">7</span><span class="sxs-lookup"><span data-stu-id="67f4c-134">7</span></span>|<span data-ttu-id="67f4c-135">指定从设备删除配置文件的用户</span><span class="sxs-lookup"><span data-stu-id="67f4c-135">Designates that the profile is removed from the device by the user</span></span>|




