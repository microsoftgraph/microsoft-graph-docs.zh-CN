---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cd0db68a21fff79ddbab924e8a1d9bd2ff2e542d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425741"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="76c3d-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="76c3d-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="76c3d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="76c3d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="76c3d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="76c3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76c3d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76c3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76c3d-107">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="76c3d-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="76c3d-108">成员</span><span class="sxs-lookup"><span data-stu-id="76c3d-108">Members</span></span>
|<span data-ttu-id="76c3d-109">成员</span><span class="sxs-lookup"><span data-stu-id="76c3d-109">Member</span></span>|<span data-ttu-id="76c3d-110">值</span><span class="sxs-lookup"><span data-stu-id="76c3d-110">Value</span></span>|<span data-ttu-id="76c3d-111">说明</span><span class="sxs-lookup"><span data-stu-id="76c3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76c3d-112">noAction</span><span class="sxs-lookup"><span data-stu-id="76c3d-112">noAction</span></span>|<span data-ttu-id="76c3d-113">0</span><span class="sxs-lookup"><span data-stu-id="76c3d-113">0</span></span>|<span data-ttu-id="76c3d-114">任何操作</span><span class="sxs-lookup"><span data-stu-id="76c3d-114">No Action</span></span>|
|<span data-ttu-id="76c3d-115">通知</span><span class="sxs-lookup"><span data-stu-id="76c3d-115">notification</span></span>|<span data-ttu-id="76c3d-116">1</span><span class="sxs-lookup"><span data-stu-id="76c3d-116">1</span></span>|<span data-ttu-id="76c3d-117">发送通知</span><span class="sxs-lookup"><span data-stu-id="76c3d-117">Send Notification</span></span>|
|<span data-ttu-id="76c3d-118">阻止</span><span class="sxs-lookup"><span data-stu-id="76c3d-118">block</span></span>|<span data-ttu-id="76c3d-119">2</span><span class="sxs-lookup"><span data-stu-id="76c3d-119">2</span></span>|<span data-ttu-id="76c3d-120">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="76c3d-120">Block the device in AAD</span></span>|
|<span data-ttu-id="76c3d-121">停用</span><span class="sxs-lookup"><span data-stu-id="76c3d-121">retire</span></span>|<span data-ttu-id="76c3d-122">3</span><span class="sxs-lookup"><span data-stu-id="76c3d-122">3</span></span>|<span data-ttu-id="76c3d-123">停用设备</span><span class="sxs-lookup"><span data-stu-id="76c3d-123">Retire the device</span></span>|
|<span data-ttu-id="76c3d-124">擦除</span><span class="sxs-lookup"><span data-stu-id="76c3d-124">wipe</span></span>|<span data-ttu-id="76c3d-125">4</span><span class="sxs-lookup"><span data-stu-id="76c3d-125">4</span></span>|<span data-ttu-id="76c3d-126">擦除设备</span><span class="sxs-lookup"><span data-stu-id="76c3d-126">Wipe the device</span></span>|
|<span data-ttu-id="76c3d-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="76c3d-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="76c3d-128">5</span><span class="sxs-lookup"><span data-stu-id="76c3d-128">5</span></span>|<span data-ttu-id="76c3d-129">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="76c3d-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="76c3d-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="76c3d-130">pushNotification</span></span>|<span data-ttu-id="76c3d-131">9</span><span class="sxs-lookup"><span data-stu-id="76c3d-131">9</span></span>|<span data-ttu-id="76c3d-132">向设备发送推送通知</span><span class="sxs-lookup"><span data-stu-id="76c3d-132">Send push notification to device</span></span>|
|<span data-ttu-id="76c3d-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="76c3d-133">remoteLock</span></span>|<span data-ttu-id="76c3d-134">10</span><span class="sxs-lookup"><span data-stu-id="76c3d-134">10</span></span>|<span data-ttu-id="76c3d-135">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="76c3d-135">Remotely lock the device</span></span>|




