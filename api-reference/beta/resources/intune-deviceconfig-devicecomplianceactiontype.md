---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9409ddebd69d8b046c522de1c3e58baabc15a2ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970617"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="2e044-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2e044-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="2e044-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2e044-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e044-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2e044-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e044-106">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="2e044-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="2e044-107">成员</span><span class="sxs-lookup"><span data-stu-id="2e044-107">Members</span></span>
|<span data-ttu-id="2e044-108">成员</span><span class="sxs-lookup"><span data-stu-id="2e044-108">Member</span></span>|<span data-ttu-id="2e044-109">值</span><span class="sxs-lookup"><span data-stu-id="2e044-109">Value</span></span>|<span data-ttu-id="2e044-110">说明</span><span class="sxs-lookup"><span data-stu-id="2e044-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e044-111">noAction</span><span class="sxs-lookup"><span data-stu-id="2e044-111">noAction</span></span>|<span data-ttu-id="2e044-112">0</span><span class="sxs-lookup"><span data-stu-id="2e044-112">0</span></span>|<span data-ttu-id="2e044-113">无操作</span><span class="sxs-lookup"><span data-stu-id="2e044-113">No Action</span></span>|
|<span data-ttu-id="2e044-114">通告</span><span class="sxs-lookup"><span data-stu-id="2e044-114">notification</span></span>|<span data-ttu-id="2e044-115">1</span><span class="sxs-lookup"><span data-stu-id="2e044-115">1</span></span>|<span data-ttu-id="2e044-116">发送通知</span><span class="sxs-lookup"><span data-stu-id="2e044-116">Send Notification</span></span>|
|<span data-ttu-id="2e044-117">数据</span><span class="sxs-lookup"><span data-stu-id="2e044-117">block</span></span>|<span data-ttu-id="2e044-118">双面</span><span class="sxs-lookup"><span data-stu-id="2e044-118">2</span></span>|<span data-ttu-id="2e044-119">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="2e044-119">Block the device in AAD</span></span>|
|<span data-ttu-id="2e044-120">注销</span><span class="sxs-lookup"><span data-stu-id="2e044-120">retire</span></span>|<span data-ttu-id="2e044-121">第三章</span><span class="sxs-lookup"><span data-stu-id="2e044-121">3</span></span>|<span data-ttu-id="2e044-122">停用设备</span><span class="sxs-lookup"><span data-stu-id="2e044-122">Retire the device</span></span>|
|<span data-ttu-id="2e044-123">擦</span><span class="sxs-lookup"><span data-stu-id="2e044-123">wipe</span></span>|<span data-ttu-id="2e044-124">4</span><span class="sxs-lookup"><span data-stu-id="2e044-124">4</span></span>|<span data-ttu-id="2e044-125">擦除设备</span><span class="sxs-lookup"><span data-stu-id="2e044-125">Wipe the device</span></span>|
|<span data-ttu-id="2e044-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="2e044-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="2e044-127">5</span><span class="sxs-lookup"><span data-stu-id="2e044-127">5</span></span>|<span data-ttu-id="2e044-128">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="2e044-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="2e044-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="2e044-129">pushNotification</span></span>|<span data-ttu-id="2e044-130">第</span><span class="sxs-lookup"><span data-stu-id="2e044-130">9</span></span>|<span data-ttu-id="2e044-131">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="2e044-131">Send push notification to device</span></span>|
|<span data-ttu-id="2e044-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="2e044-132">remoteLock</span></span>|<span data-ttu-id="2e044-133">10 </span><span class="sxs-lookup"><span data-stu-id="2e044-133">10</span></span>|<span data-ttu-id="2e044-134">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="2e044-134">Remotely lock the device</span></span>|





