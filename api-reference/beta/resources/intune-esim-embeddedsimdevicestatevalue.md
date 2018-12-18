---
title: embeddedSIMDeviceStateValue 枚举类型
description: 介绍为嵌入 SIM 激活代码的各种状态。
author: tfitzmac
ms.openlocfilehash: 51e550669d9cd29d7d5bb246fe2cba017b02187c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320592"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="5474a-103">embeddedSIMDeviceStateValue 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5474a-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="5474a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5474a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5474a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5474a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5474a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5474a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5474a-107">介绍为嵌入 SIM 激活代码的各种状态。</span><span class="sxs-lookup"><span data-stu-id="5474a-107">Describes the various states for an embedded SIM activation code.</span></span>
## <a name="members"></a><span data-ttu-id="5474a-108">成员</span><span class="sxs-lookup"><span data-stu-id="5474a-108">Members</span></span>
|<span data-ttu-id="5474a-109">成员</span><span class="sxs-lookup"><span data-stu-id="5474a-109">Member</span></span>|<span data-ttu-id="5474a-110">值</span><span class="sxs-lookup"><span data-stu-id="5474a-110">Value</span></span>|<span data-ttu-id="5474a-111">说明</span><span class="sxs-lookup"><span data-stu-id="5474a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5474a-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="5474a-112">notEvaluated</span></span>|<span data-ttu-id="5474a-113">0</span><span class="sxs-lookup"><span data-stu-id="5474a-113">0</span></span>|<span data-ttu-id="5474a-114">指定嵌入的 SIM 激活代码可用，并且可以分配给设备。</span><span class="sxs-lookup"><span data-stu-id="5474a-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="5474a-115">failed</span><span class="sxs-lookup"><span data-stu-id="5474a-115">failed</span></span>|<span data-ttu-id="5474a-116">1</span><span class="sxs-lookup"><span data-stu-id="5474a-116">1</span></span>|<span data-ttu-id="5474a-117">指定 Intune 服务未能向设备提供此配置文件。</span><span class="sxs-lookup"><span data-stu-id="5474a-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="5474a-118">安装</span><span class="sxs-lookup"><span data-stu-id="5474a-118">installing</span></span>|<span data-ttu-id="5474a-119">2</span><span class="sxs-lookup"><span data-stu-id="5474a-119">2</span></span>|<span data-ttu-id="5474a-120">指定的嵌入式的 SIM 激活代码已分配给设备和设备安装令牌。</span><span class="sxs-lookup"><span data-stu-id="5474a-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="5474a-121">安装</span><span class="sxs-lookup"><span data-stu-id="5474a-121">installed</span></span>|<span data-ttu-id="5474a-122">3</span><span class="sxs-lookup"><span data-stu-id="5474a-122">3</span></span>|<span data-ttu-id="5474a-123">指定已成功目标设备上安装的嵌入的 SIM 激活代码。</span><span class="sxs-lookup"><span data-stu-id="5474a-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="5474a-124">删除</span><span class="sxs-lookup"><span data-stu-id="5474a-124">deleting</span></span>|<span data-ttu-id="5474a-125">4</span><span class="sxs-lookup"><span data-stu-id="5474a-125">4</span></span>|<span data-ttu-id="5474a-126">指定 Intune 服务尝试从设备中删除配置文件。</span><span class="sxs-lookup"><span data-stu-id="5474a-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="5474a-127">error</span><span class="sxs-lookup"><span data-stu-id="5474a-127">error</span></span>|<span data-ttu-id="5474a-128">5</span><span class="sxs-lookup"><span data-stu-id="5474a-128">5</span></span>|<span data-ttu-id="5474a-129">指定存在与此配置文件的错误。</span><span class="sxs-lookup"><span data-stu-id="5474a-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="5474a-130">deleted</span><span class="sxs-lookup"><span data-stu-id="5474a-130">deleted</span></span>|<span data-ttu-id="5474a-131">6</span><span class="sxs-lookup"><span data-stu-id="5474a-131">6</span></span>|<span data-ttu-id="5474a-132">指定从设备中删除配置文件。</span><span class="sxs-lookup"><span data-stu-id="5474a-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="5474a-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="5474a-133">removedByUser</span></span>|<span data-ttu-id="5474a-134">7</span><span class="sxs-lookup"><span data-stu-id="5474a-134">7</span></span>|<span data-ttu-id="5474a-135">指定从设备删除配置文件的用户</span><span class="sxs-lookup"><span data-stu-id="5474a-135">Designates that the profile is removed from the device by the user</span></span>|





