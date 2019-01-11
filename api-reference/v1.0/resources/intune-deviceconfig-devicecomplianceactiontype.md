---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 92e43378f119a5e1a10604babb5ad23b2dfddf3b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851434"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="a4c3f-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a4c3f-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="a4c3f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a4c3f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4c3f-105">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="a4c3f-105">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="a4c3f-106">成员</span><span class="sxs-lookup"><span data-stu-id="a4c3f-106">Members</span></span>
|<span data-ttu-id="a4c3f-107">成员</span><span class="sxs-lookup"><span data-stu-id="a4c3f-107">Member</span></span>|<span data-ttu-id="a4c3f-108">值</span><span class="sxs-lookup"><span data-stu-id="a4c3f-108">Value</span></span>|<span data-ttu-id="a4c3f-109">Description</span><span class="sxs-lookup"><span data-stu-id="a4c3f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4c3f-110">noAction</span><span class="sxs-lookup"><span data-stu-id="a4c3f-110">noAction</span></span>|<span data-ttu-id="a4c3f-111">0</span><span class="sxs-lookup"><span data-stu-id="a4c3f-111">0</span></span>|<span data-ttu-id="a4c3f-112">任何操作</span><span class="sxs-lookup"><span data-stu-id="a4c3f-112">No Action</span></span>|
|<span data-ttu-id="a4c3f-113">通知</span><span class="sxs-lookup"><span data-stu-id="a4c3f-113">notification</span></span>|<span data-ttu-id="a4c3f-114">1</span><span class="sxs-lookup"><span data-stu-id="a4c3f-114">1</span></span>|<span data-ttu-id="a4c3f-115">发送通知</span><span class="sxs-lookup"><span data-stu-id="a4c3f-115">Send Notification</span></span>|
|<span data-ttu-id="a4c3f-116">阻止</span><span class="sxs-lookup"><span data-stu-id="a4c3f-116">block</span></span>|<span data-ttu-id="a4c3f-117">2</span><span class="sxs-lookup"><span data-stu-id="a4c3f-117">2</span></span>|<span data-ttu-id="a4c3f-118">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="a4c3f-118">Block the device in AAD</span></span>|
|<span data-ttu-id="a4c3f-119">停用</span><span class="sxs-lookup"><span data-stu-id="a4c3f-119">retire</span></span>|<span data-ttu-id="a4c3f-120">3</span><span class="sxs-lookup"><span data-stu-id="a4c3f-120">3</span></span>|<span data-ttu-id="a4c3f-121">停用设备</span><span class="sxs-lookup"><span data-stu-id="a4c3f-121">Retire the device</span></span>|
|<span data-ttu-id="a4c3f-122">擦除</span><span class="sxs-lookup"><span data-stu-id="a4c3f-122">wipe</span></span>|<span data-ttu-id="a4c3f-123">4</span><span class="sxs-lookup"><span data-stu-id="a4c3f-123">4</span></span>|<span data-ttu-id="a4c3f-124">擦除设备</span><span class="sxs-lookup"><span data-stu-id="a4c3f-124">Wipe the device</span></span>|
|<span data-ttu-id="a4c3f-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="a4c3f-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="a4c3f-126">5</span><span class="sxs-lookup"><span data-stu-id="a4c3f-126">5</span></span>|<span data-ttu-id="a4c3f-127">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="a4c3f-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="a4c3f-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="a4c3f-128">pushNotification</span></span>|<span data-ttu-id="a4c3f-129">9</span><span class="sxs-lookup"><span data-stu-id="a4c3f-129">9</span></span>|<span data-ttu-id="a4c3f-130">向设备发送推送通知</span><span class="sxs-lookup"><span data-stu-id="a4c3f-130">Send push notification to device</span></span>|



