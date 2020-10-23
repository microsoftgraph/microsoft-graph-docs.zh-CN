---
title: embeddedSIMDeviceStateValue 枚举类型
description: 描述嵌入的 SIM 激活代码的各种状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 27e7b9e343d751f0417b7bd5dce3d526c93f131f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736126"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="0b870-103">embeddedSIMDeviceStateValue 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0b870-103">embeddedSIMDeviceStateValue enum type</span></span>

<span data-ttu-id="0b870-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b870-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b870-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0b870-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b870-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b870-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b870-107">描述嵌入的 SIM 激活代码的各种状态。</span><span class="sxs-lookup"><span data-stu-id="0b870-107">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="0b870-108">成员</span><span class="sxs-lookup"><span data-stu-id="0b870-108">Members</span></span>
|<span data-ttu-id="0b870-109">成员</span><span class="sxs-lookup"><span data-stu-id="0b870-109">Member</span></span>|<span data-ttu-id="0b870-110">值</span><span class="sxs-lookup"><span data-stu-id="0b870-110">Value</span></span>|<span data-ttu-id="0b870-111">说明</span><span class="sxs-lookup"><span data-stu-id="0b870-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b870-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="0b870-112">notEvaluated</span></span>|<span data-ttu-id="0b870-113">0</span><span class="sxs-lookup"><span data-stu-id="0b870-113">0</span></span>|<span data-ttu-id="0b870-114">指明嵌入的 SIM 激活代码是免费的，可以分配给设备。</span><span class="sxs-lookup"><span data-stu-id="0b870-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="0b870-115">未能</span><span class="sxs-lookup"><span data-stu-id="0b870-115">failed</span></span>|<span data-ttu-id="0b870-116">1</span><span class="sxs-lookup"><span data-stu-id="0b870-116">1</span></span>|<span data-ttu-id="0b870-117">指定 Intune 服务无法将此配置文件传递给设备。</span><span class="sxs-lookup"><span data-stu-id="0b870-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="0b870-118">安装</span><span class="sxs-lookup"><span data-stu-id="0b870-118">installing</span></span>|<span data-ttu-id="0b870-119">双面</span><span class="sxs-lookup"><span data-stu-id="0b870-119">2</span></span>|<span data-ttu-id="0b870-120">指定已将嵌入的 SIM 激活代码分配给设备，并且设备正在安装令牌。</span><span class="sxs-lookup"><span data-stu-id="0b870-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="0b870-121">了</span><span class="sxs-lookup"><span data-stu-id="0b870-121">installed</span></span>|<span data-ttu-id="0b870-122">第三章</span><span class="sxs-lookup"><span data-stu-id="0b870-122">3</span></span>|<span data-ttu-id="0b870-123">指定已在目标设备上成功安装嵌入的 SIM 激活代码。</span><span class="sxs-lookup"><span data-stu-id="0b870-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="0b870-124">删除</span><span class="sxs-lookup"><span data-stu-id="0b870-124">deleting</span></span>|<span data-ttu-id="0b870-125">4 </span><span class="sxs-lookup"><span data-stu-id="0b870-125">4</span></span>|<span data-ttu-id="0b870-126">指定 Intune 服务正在尝试从设备中删除配置文件。</span><span class="sxs-lookup"><span data-stu-id="0b870-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="0b870-127">error</span><span class="sxs-lookup"><span data-stu-id="0b870-127">error</span></span>|<span data-ttu-id="0b870-128">5 </span><span class="sxs-lookup"><span data-stu-id="0b870-128">5</span></span>|<span data-ttu-id="0b870-129">指定此配置文件存在错误。</span><span class="sxs-lookup"><span data-stu-id="0b870-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="0b870-130">deleted</span><span class="sxs-lookup"><span data-stu-id="0b870-130">deleted</span></span>|<span data-ttu-id="0b870-131">6 </span><span class="sxs-lookup"><span data-stu-id="0b870-131">6</span></span>|<span data-ttu-id="0b870-132">指定将配置文件从设备中删除。</span><span class="sxs-lookup"><span data-stu-id="0b870-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="0b870-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="0b870-133">removedByUser</span></span>|<span data-ttu-id="0b870-134">7 </span><span class="sxs-lookup"><span data-stu-id="0b870-134">7</span></span>|<span data-ttu-id="0b870-135">指定用户从设备中删除配置文件</span><span class="sxs-lookup"><span data-stu-id="0b870-135">Designates that the profile is removed from the device by the user</span></span>|





