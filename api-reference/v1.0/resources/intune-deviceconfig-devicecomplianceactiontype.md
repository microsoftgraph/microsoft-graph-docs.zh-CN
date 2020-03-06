---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2a8b74f0bb668a9354bc2d68d21a7c45e52d1c06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530854"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="1df01-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1df01-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="1df01-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1df01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1df01-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1df01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1df01-106">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="1df01-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="1df01-107">成员</span><span class="sxs-lookup"><span data-stu-id="1df01-107">Members</span></span>
|<span data-ttu-id="1df01-108">成员</span><span class="sxs-lookup"><span data-stu-id="1df01-108">Member</span></span>|<span data-ttu-id="1df01-109">值</span><span class="sxs-lookup"><span data-stu-id="1df01-109">Value</span></span>|<span data-ttu-id="1df01-110">说明</span><span class="sxs-lookup"><span data-stu-id="1df01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1df01-111">noAction</span><span class="sxs-lookup"><span data-stu-id="1df01-111">noAction</span></span>|<span data-ttu-id="1df01-112">0</span><span class="sxs-lookup"><span data-stu-id="1df01-112">0</span></span>|<span data-ttu-id="1df01-113">无操作</span><span class="sxs-lookup"><span data-stu-id="1df01-113">No Action</span></span>|
|<span data-ttu-id="1df01-114">通告</span><span class="sxs-lookup"><span data-stu-id="1df01-114">notification</span></span>|<span data-ttu-id="1df01-115">1 </span><span class="sxs-lookup"><span data-stu-id="1df01-115">1</span></span>|<span data-ttu-id="1df01-116">发送通知</span><span class="sxs-lookup"><span data-stu-id="1df01-116">Send Notification</span></span>|
|<span data-ttu-id="1df01-117">数据</span><span class="sxs-lookup"><span data-stu-id="1df01-117">block</span></span>|<span data-ttu-id="1df01-118">2 </span><span class="sxs-lookup"><span data-stu-id="1df01-118">2</span></span>|<span data-ttu-id="1df01-119">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="1df01-119">Block the device in AAD</span></span>|
|<span data-ttu-id="1df01-120">注销</span><span class="sxs-lookup"><span data-stu-id="1df01-120">retire</span></span>|<span data-ttu-id="1df01-121">3 </span><span class="sxs-lookup"><span data-stu-id="1df01-121">3</span></span>|<span data-ttu-id="1df01-122">停用设备</span><span class="sxs-lookup"><span data-stu-id="1df01-122">Retire the device</span></span>|
|<span data-ttu-id="1df01-123">擦</span><span class="sxs-lookup"><span data-stu-id="1df01-123">wipe</span></span>|<span data-ttu-id="1df01-124">4 </span><span class="sxs-lookup"><span data-stu-id="1df01-124">4</span></span>|<span data-ttu-id="1df01-125">擦除设备</span><span class="sxs-lookup"><span data-stu-id="1df01-125">Wipe the device</span></span>|
|<span data-ttu-id="1df01-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="1df01-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="1df01-127">5 </span><span class="sxs-lookup"><span data-stu-id="1df01-127">5</span></span>|<span data-ttu-id="1df01-128">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="1df01-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="1df01-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="1df01-129">pushNotification</span></span>|<span data-ttu-id="1df01-130">9 </span><span class="sxs-lookup"><span data-stu-id="1df01-130">9</span></span>|<span data-ttu-id="1df01-131">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="1df01-131">Send push notification to device</span></span>|




