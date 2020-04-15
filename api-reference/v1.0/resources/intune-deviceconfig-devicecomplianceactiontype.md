---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e9b44df925cfad240202ad207ddb883b61d6be18
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448958"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="6d215-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6d215-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="6d215-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d215-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d215-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d215-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d215-106">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="6d215-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="6d215-107">成员</span><span class="sxs-lookup"><span data-stu-id="6d215-107">Members</span></span>
|<span data-ttu-id="6d215-108">成员</span><span class="sxs-lookup"><span data-stu-id="6d215-108">Member</span></span>|<span data-ttu-id="6d215-109">值</span><span class="sxs-lookup"><span data-stu-id="6d215-109">Value</span></span>|<span data-ttu-id="6d215-110">说明</span><span class="sxs-lookup"><span data-stu-id="6d215-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d215-111">noAction</span><span class="sxs-lookup"><span data-stu-id="6d215-111">noAction</span></span>|<span data-ttu-id="6d215-112">0</span><span class="sxs-lookup"><span data-stu-id="6d215-112">0</span></span>|<span data-ttu-id="6d215-113">无操作</span><span class="sxs-lookup"><span data-stu-id="6d215-113">No Action</span></span>|
|<span data-ttu-id="6d215-114">通告</span><span class="sxs-lookup"><span data-stu-id="6d215-114">notification</span></span>|<span data-ttu-id="6d215-115">1</span><span class="sxs-lookup"><span data-stu-id="6d215-115">1</span></span>|<span data-ttu-id="6d215-116">发送通知</span><span class="sxs-lookup"><span data-stu-id="6d215-116">Send Notification</span></span>|
|<span data-ttu-id="6d215-117">数据</span><span class="sxs-lookup"><span data-stu-id="6d215-117">block</span></span>|<span data-ttu-id="6d215-118">双面</span><span class="sxs-lookup"><span data-stu-id="6d215-118">2</span></span>|<span data-ttu-id="6d215-119">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="6d215-119">Block the device in AAD</span></span>|
|<span data-ttu-id="6d215-120">注销</span><span class="sxs-lookup"><span data-stu-id="6d215-120">retire</span></span>|<span data-ttu-id="6d215-121">第三章</span><span class="sxs-lookup"><span data-stu-id="6d215-121">3</span></span>|<span data-ttu-id="6d215-122">停用设备</span><span class="sxs-lookup"><span data-stu-id="6d215-122">Retire the device</span></span>|
|<span data-ttu-id="6d215-123">擦</span><span class="sxs-lookup"><span data-stu-id="6d215-123">wipe</span></span>|<span data-ttu-id="6d215-124">4 </span><span class="sxs-lookup"><span data-stu-id="6d215-124">4</span></span>|<span data-ttu-id="6d215-125">擦除设备</span><span class="sxs-lookup"><span data-stu-id="6d215-125">Wipe the device</span></span>|
|<span data-ttu-id="6d215-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="6d215-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="6d215-127">5 </span><span class="sxs-lookup"><span data-stu-id="6d215-127">5</span></span>|<span data-ttu-id="6d215-128">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="6d215-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="6d215-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="6d215-129">pushNotification</span></span>|<span data-ttu-id="6d215-130">9 </span><span class="sxs-lookup"><span data-stu-id="6d215-130">9</span></span>|<span data-ttu-id="6d215-131">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="6d215-131">Send push notification to device</span></span>|







