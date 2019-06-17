---
title: embeddedSIMDeviceStateValue 枚举类型
description: 描述嵌入的 SIM 激活代码的各种状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a22641d40b05fa41cc9542df5237a2e9e278a401
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987298"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="9fceb-103">embeddedSIMDeviceStateValue 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9fceb-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="9fceb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9fceb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fceb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fceb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fceb-106">描述嵌入的 SIM 激活代码的各种状态。</span><span class="sxs-lookup"><span data-stu-id="9fceb-106">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="9fceb-107">成员</span><span class="sxs-lookup"><span data-stu-id="9fceb-107">Members</span></span>
|<span data-ttu-id="9fceb-108">成员</span><span class="sxs-lookup"><span data-stu-id="9fceb-108">Member</span></span>|<span data-ttu-id="9fceb-109">值</span><span class="sxs-lookup"><span data-stu-id="9fceb-109">Value</span></span>|<span data-ttu-id="9fceb-110">说明</span><span class="sxs-lookup"><span data-stu-id="9fceb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fceb-111">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="9fceb-111">notEvaluated</span></span>|<span data-ttu-id="9fceb-112">0</span><span class="sxs-lookup"><span data-stu-id="9fceb-112">0</span></span>|<span data-ttu-id="9fceb-113">指明嵌入的 SIM 激活代码是免费的, 可以分配给设备。</span><span class="sxs-lookup"><span data-stu-id="9fceb-113">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="9fceb-114">未能</span><span class="sxs-lookup"><span data-stu-id="9fceb-114">failed</span></span>|<span data-ttu-id="9fceb-115">1</span><span class="sxs-lookup"><span data-stu-id="9fceb-115">1</span></span>|<span data-ttu-id="9fceb-116">指定 Intune 服务无法将此配置文件传递给设备。</span><span class="sxs-lookup"><span data-stu-id="9fceb-116">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="9fceb-117">安装</span><span class="sxs-lookup"><span data-stu-id="9fceb-117">installing</span></span>|<span data-ttu-id="9fceb-118">双面</span><span class="sxs-lookup"><span data-stu-id="9fceb-118">2</span></span>|<span data-ttu-id="9fceb-119">指定已将嵌入的 SIM 激活代码分配给设备, 并且设备正在安装令牌。</span><span class="sxs-lookup"><span data-stu-id="9fceb-119">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="9fceb-120">了</span><span class="sxs-lookup"><span data-stu-id="9fceb-120">installed</span></span>|<span data-ttu-id="9fceb-121">第三章</span><span class="sxs-lookup"><span data-stu-id="9fceb-121">3</span></span>|<span data-ttu-id="9fceb-122">指定已在目标设备上成功安装嵌入的 SIM 激活代码。</span><span class="sxs-lookup"><span data-stu-id="9fceb-122">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="9fceb-123">删除</span><span class="sxs-lookup"><span data-stu-id="9fceb-123">deleting</span></span>|<span data-ttu-id="9fceb-124">4</span><span class="sxs-lookup"><span data-stu-id="9fceb-124">4</span></span>|<span data-ttu-id="9fceb-125">指定 Intune 服务正在尝试从设备中删除配置文件。</span><span class="sxs-lookup"><span data-stu-id="9fceb-125">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="9fceb-126">error</span><span class="sxs-lookup"><span data-stu-id="9fceb-126">error</span></span>|<span data-ttu-id="9fceb-127">5</span><span class="sxs-lookup"><span data-stu-id="9fceb-127">5</span></span>|<span data-ttu-id="9fceb-128">指定此配置文件存在错误。</span><span class="sxs-lookup"><span data-stu-id="9fceb-128">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="9fceb-129">deleted</span><span class="sxs-lookup"><span data-stu-id="9fceb-129">deleted</span></span>|<span data-ttu-id="9fceb-130">型</span><span class="sxs-lookup"><span data-stu-id="9fceb-130">6</span></span>|<span data-ttu-id="9fceb-131">指定将配置文件从设备中删除。</span><span class="sxs-lookup"><span data-stu-id="9fceb-131">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="9fceb-132">removedByUser</span><span class="sxs-lookup"><span data-stu-id="9fceb-132">removedByUser</span></span>|<span data-ttu-id="9fceb-133">步</span><span class="sxs-lookup"><span data-stu-id="9fceb-133">7</span></span>|<span data-ttu-id="9fceb-134">指定用户从设备中删除配置文件</span><span class="sxs-lookup"><span data-stu-id="9fceb-134">Designates that the profile is removed from the device by the user</span></span>|





