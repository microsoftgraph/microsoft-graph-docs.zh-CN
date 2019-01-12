---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8d725213790260ece51c02bb81f2394fc8602095
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917340"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="464ba-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="464ba-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="464ba-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="464ba-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="464ba-105">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="464ba-105">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="464ba-106">成员</span><span class="sxs-lookup"><span data-stu-id="464ba-106">Members</span></span>
|<span data-ttu-id="464ba-107">成员</span><span class="sxs-lookup"><span data-stu-id="464ba-107">Member</span></span>|<span data-ttu-id="464ba-108">值</span><span class="sxs-lookup"><span data-stu-id="464ba-108">Value</span></span>|<span data-ttu-id="464ba-109">Description</span><span class="sxs-lookup"><span data-stu-id="464ba-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="464ba-110">noAction</span><span class="sxs-lookup"><span data-stu-id="464ba-110">noAction</span></span>|<span data-ttu-id="464ba-111">0</span><span class="sxs-lookup"><span data-stu-id="464ba-111">0</span></span>|<span data-ttu-id="464ba-112">任何操作</span><span class="sxs-lookup"><span data-stu-id="464ba-112">No Action</span></span>|
|<span data-ttu-id="464ba-113">通知</span><span class="sxs-lookup"><span data-stu-id="464ba-113">notification</span></span>|<span data-ttu-id="464ba-114">1</span><span class="sxs-lookup"><span data-stu-id="464ba-114">1</span></span>|<span data-ttu-id="464ba-115">发送通知</span><span class="sxs-lookup"><span data-stu-id="464ba-115">Send Notification</span></span>|
|<span data-ttu-id="464ba-116">阻止</span><span class="sxs-lookup"><span data-stu-id="464ba-116">block</span></span>|<span data-ttu-id="464ba-117">2</span><span class="sxs-lookup"><span data-stu-id="464ba-117">2</span></span>|<span data-ttu-id="464ba-118">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="464ba-118">Block the device in AAD</span></span>|
|<span data-ttu-id="464ba-119">停用</span><span class="sxs-lookup"><span data-stu-id="464ba-119">retire</span></span>|<span data-ttu-id="464ba-120">3</span><span class="sxs-lookup"><span data-stu-id="464ba-120">3</span></span>|<span data-ttu-id="464ba-121">停用设备</span><span class="sxs-lookup"><span data-stu-id="464ba-121">Retire the device</span></span>|
|<span data-ttu-id="464ba-122">擦除</span><span class="sxs-lookup"><span data-stu-id="464ba-122">wipe</span></span>|<span data-ttu-id="464ba-123">4</span><span class="sxs-lookup"><span data-stu-id="464ba-123">4</span></span>|<span data-ttu-id="464ba-124">擦除设备</span><span class="sxs-lookup"><span data-stu-id="464ba-124">Wipe the device</span></span>|
|<span data-ttu-id="464ba-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="464ba-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="464ba-126">5</span><span class="sxs-lookup"><span data-stu-id="464ba-126">5</span></span>|<span data-ttu-id="464ba-127">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="464ba-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="464ba-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="464ba-128">pushNotification</span></span>|<span data-ttu-id="464ba-129">9</span><span class="sxs-lookup"><span data-stu-id="464ba-129">9</span></span>|<span data-ttu-id="464ba-130">向设备发送推送通知</span><span class="sxs-lookup"><span data-stu-id="464ba-130">Send push notification to device</span></span>|



