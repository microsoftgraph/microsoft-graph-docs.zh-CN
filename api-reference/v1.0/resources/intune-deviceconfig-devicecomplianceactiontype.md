---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fcfad0e76f1977f9353d63a1367cdef35c76d69e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041461"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="c3eec-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c3eec-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="c3eec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3eec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3eec-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3eec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3eec-106">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="c3eec-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="c3eec-107">成员</span><span class="sxs-lookup"><span data-stu-id="c3eec-107">Members</span></span>
|<span data-ttu-id="c3eec-108">成员</span><span class="sxs-lookup"><span data-stu-id="c3eec-108">Member</span></span>|<span data-ttu-id="c3eec-109">值</span><span class="sxs-lookup"><span data-stu-id="c3eec-109">Value</span></span>|<span data-ttu-id="c3eec-110">说明</span><span class="sxs-lookup"><span data-stu-id="c3eec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3eec-111">noAction</span><span class="sxs-lookup"><span data-stu-id="c3eec-111">noAction</span></span>|<span data-ttu-id="c3eec-112">0</span><span class="sxs-lookup"><span data-stu-id="c3eec-112">0</span></span>|<span data-ttu-id="c3eec-113">无操作</span><span class="sxs-lookup"><span data-stu-id="c3eec-113">No Action</span></span>|
|<span data-ttu-id="c3eec-114">通告</span><span class="sxs-lookup"><span data-stu-id="c3eec-114">notification</span></span>|<span data-ttu-id="c3eec-115">1 </span><span class="sxs-lookup"><span data-stu-id="c3eec-115">1</span></span>|<span data-ttu-id="c3eec-116">发送通知</span><span class="sxs-lookup"><span data-stu-id="c3eec-116">Send Notification</span></span>|
|<span data-ttu-id="c3eec-117">数据</span><span class="sxs-lookup"><span data-stu-id="c3eec-117">block</span></span>|<span data-ttu-id="c3eec-118">2 </span><span class="sxs-lookup"><span data-stu-id="c3eec-118">2</span></span>|<span data-ttu-id="c3eec-119">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="c3eec-119">Block the device in AAD</span></span>|
|<span data-ttu-id="c3eec-120">注销</span><span class="sxs-lookup"><span data-stu-id="c3eec-120">retire</span></span>|<span data-ttu-id="c3eec-121">第三章</span><span class="sxs-lookup"><span data-stu-id="c3eec-121">3</span></span>|<span data-ttu-id="c3eec-122">停用设备</span><span class="sxs-lookup"><span data-stu-id="c3eec-122">Retire the device</span></span>|
|<span data-ttu-id="c3eec-123">擦</span><span class="sxs-lookup"><span data-stu-id="c3eec-123">wipe</span></span>|<span data-ttu-id="c3eec-124">4 </span><span class="sxs-lookup"><span data-stu-id="c3eec-124">4</span></span>|<span data-ttu-id="c3eec-125">擦除设备</span><span class="sxs-lookup"><span data-stu-id="c3eec-125">Wipe the device</span></span>|
|<span data-ttu-id="c3eec-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="c3eec-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="c3eec-127">5 </span><span class="sxs-lookup"><span data-stu-id="c3eec-127">5</span></span>|<span data-ttu-id="c3eec-128">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="c3eec-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="c3eec-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="c3eec-129">pushNotification</span></span>|<span data-ttu-id="c3eec-130">9 </span><span class="sxs-lookup"><span data-stu-id="c3eec-130">9</span></span>|<span data-ttu-id="c3eec-131">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="c3eec-131">Send push notification to device</span></span>|









