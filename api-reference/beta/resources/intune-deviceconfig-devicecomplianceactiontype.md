---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4ebf4df22787d19e5718ebd2099cd81af3925271
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793357"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="0a296-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0a296-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="0a296-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0a296-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a296-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a296-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a296-106">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="0a296-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="0a296-107">成员</span><span class="sxs-lookup"><span data-stu-id="0a296-107">Members</span></span>
|<span data-ttu-id="0a296-108">成员</span><span class="sxs-lookup"><span data-stu-id="0a296-108">Member</span></span>|<span data-ttu-id="0a296-109">值</span><span class="sxs-lookup"><span data-stu-id="0a296-109">Value</span></span>|<span data-ttu-id="0a296-110">说明</span><span class="sxs-lookup"><span data-stu-id="0a296-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a296-111">noAction</span><span class="sxs-lookup"><span data-stu-id="0a296-111">noAction</span></span>|<span data-ttu-id="0a296-112">0</span><span class="sxs-lookup"><span data-stu-id="0a296-112">0</span></span>|<span data-ttu-id="0a296-113">无操作</span><span class="sxs-lookup"><span data-stu-id="0a296-113">No Action</span></span>|
|<span data-ttu-id="0a296-114">通告</span><span class="sxs-lookup"><span data-stu-id="0a296-114">notification</span></span>|<span data-ttu-id="0a296-115">1</span><span class="sxs-lookup"><span data-stu-id="0a296-115">1</span></span>|<span data-ttu-id="0a296-116">发送通知</span><span class="sxs-lookup"><span data-stu-id="0a296-116">Send Notification</span></span>|
|<span data-ttu-id="0a296-117">数据</span><span class="sxs-lookup"><span data-stu-id="0a296-117">block</span></span>|<span data-ttu-id="0a296-118">双面</span><span class="sxs-lookup"><span data-stu-id="0a296-118">2</span></span>|<span data-ttu-id="0a296-119">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="0a296-119">Block the device in AAD</span></span>|
|<span data-ttu-id="0a296-120">注销</span><span class="sxs-lookup"><span data-stu-id="0a296-120">retire</span></span>|<span data-ttu-id="0a296-121">第三章</span><span class="sxs-lookup"><span data-stu-id="0a296-121">3</span></span>|<span data-ttu-id="0a296-122">停用设备</span><span class="sxs-lookup"><span data-stu-id="0a296-122">Retire the device</span></span>|
|<span data-ttu-id="0a296-123">擦</span><span class="sxs-lookup"><span data-stu-id="0a296-123">wipe</span></span>|<span data-ttu-id="0a296-124">4 </span><span class="sxs-lookup"><span data-stu-id="0a296-124">4</span></span>|<span data-ttu-id="0a296-125">擦除设备</span><span class="sxs-lookup"><span data-stu-id="0a296-125">Wipe the device</span></span>|
|<span data-ttu-id="0a296-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="0a296-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="0a296-127">5 </span><span class="sxs-lookup"><span data-stu-id="0a296-127">5</span></span>|<span data-ttu-id="0a296-128">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="0a296-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="0a296-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="0a296-129">pushNotification</span></span>|<span data-ttu-id="0a296-130">9 </span><span class="sxs-lookup"><span data-stu-id="0a296-130">9</span></span>|<span data-ttu-id="0a296-131">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="0a296-131">Send push notification to device</span></span>|
|<span data-ttu-id="0a296-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="0a296-132">remoteLock</span></span>|<span data-ttu-id="0a296-133">10 </span><span class="sxs-lookup"><span data-stu-id="0a296-133">10</span></span>|<span data-ttu-id="0a296-134">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="0a296-134">Remotely lock the device</span></span>|



