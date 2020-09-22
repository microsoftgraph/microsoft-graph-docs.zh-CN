---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f441179e425f341d55eaee02525894aec53e487c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085043"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="a3859-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a3859-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="a3859-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3859-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3859-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3859-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3859-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3859-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3859-107">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="a3859-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="a3859-108">成员</span><span class="sxs-lookup"><span data-stu-id="a3859-108">Members</span></span>
|<span data-ttu-id="a3859-109">成员</span><span class="sxs-lookup"><span data-stu-id="a3859-109">Member</span></span>|<span data-ttu-id="a3859-110">值</span><span class="sxs-lookup"><span data-stu-id="a3859-110">Value</span></span>|<span data-ttu-id="a3859-111">说明</span><span class="sxs-lookup"><span data-stu-id="a3859-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3859-112">noAction</span><span class="sxs-lookup"><span data-stu-id="a3859-112">noAction</span></span>|<span data-ttu-id="a3859-113">0</span><span class="sxs-lookup"><span data-stu-id="a3859-113">0</span></span>|<span data-ttu-id="a3859-114">无操作</span><span class="sxs-lookup"><span data-stu-id="a3859-114">No Action</span></span>|
|<span data-ttu-id="a3859-115">通告</span><span class="sxs-lookup"><span data-stu-id="a3859-115">notification</span></span>|<span data-ttu-id="a3859-116">1 </span><span class="sxs-lookup"><span data-stu-id="a3859-116">1</span></span>|<span data-ttu-id="a3859-117">发送通知</span><span class="sxs-lookup"><span data-stu-id="a3859-117">Send Notification</span></span>|
|<span data-ttu-id="a3859-118">数据</span><span class="sxs-lookup"><span data-stu-id="a3859-118">block</span></span>|<span data-ttu-id="a3859-119">2 </span><span class="sxs-lookup"><span data-stu-id="a3859-119">2</span></span>|<span data-ttu-id="a3859-120">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="a3859-120">Block the device in AAD</span></span>|
|<span data-ttu-id="a3859-121">注销</span><span class="sxs-lookup"><span data-stu-id="a3859-121">retire</span></span>|<span data-ttu-id="a3859-122">第三章</span><span class="sxs-lookup"><span data-stu-id="a3859-122">3</span></span>|<span data-ttu-id="a3859-123">停用设备</span><span class="sxs-lookup"><span data-stu-id="a3859-123">Retire the device</span></span>|
|<span data-ttu-id="a3859-124">擦</span><span class="sxs-lookup"><span data-stu-id="a3859-124">wipe</span></span>|<span data-ttu-id="a3859-125">4 </span><span class="sxs-lookup"><span data-stu-id="a3859-125">4</span></span>|<span data-ttu-id="a3859-126">擦除设备</span><span class="sxs-lookup"><span data-stu-id="a3859-126">Wipe the device</span></span>|
|<span data-ttu-id="a3859-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="a3859-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="a3859-128">5 </span><span class="sxs-lookup"><span data-stu-id="a3859-128">5</span></span>|<span data-ttu-id="a3859-129">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="a3859-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="a3859-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="a3859-130">pushNotification</span></span>|<span data-ttu-id="a3859-131">9 </span><span class="sxs-lookup"><span data-stu-id="a3859-131">9</span></span>|<span data-ttu-id="a3859-132">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="a3859-132">Send push notification to device</span></span>|
|<span data-ttu-id="a3859-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="a3859-133">remoteLock</span></span>|<span data-ttu-id="a3859-134">10 </span><span class="sxs-lookup"><span data-stu-id="a3859-134">10</span></span>|<span data-ttu-id="a3859-135">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="a3859-135">Remotely lock the device</span></span>|






