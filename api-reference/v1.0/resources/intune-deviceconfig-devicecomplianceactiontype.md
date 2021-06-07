---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f4b4a20776eb24c3f2af00557b8fdbb88c60ca65
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751417"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="978a0-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="978a0-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="978a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="978a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="978a0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="978a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="978a0-106">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="978a0-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="978a0-107">成员</span><span class="sxs-lookup"><span data-stu-id="978a0-107">Members</span></span>
|<span data-ttu-id="978a0-108">成员</span><span class="sxs-lookup"><span data-stu-id="978a0-108">Member</span></span>|<span data-ttu-id="978a0-109">值</span><span class="sxs-lookup"><span data-stu-id="978a0-109">Value</span></span>|<span data-ttu-id="978a0-110">Description</span><span class="sxs-lookup"><span data-stu-id="978a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="978a0-111">noAction</span><span class="sxs-lookup"><span data-stu-id="978a0-111">noAction</span></span>|<span data-ttu-id="978a0-112">0</span><span class="sxs-lookup"><span data-stu-id="978a0-112">0</span></span>|<span data-ttu-id="978a0-113">无操作</span><span class="sxs-lookup"><span data-stu-id="978a0-113">No Action</span></span>|
|<span data-ttu-id="978a0-114">通知</span><span class="sxs-lookup"><span data-stu-id="978a0-114">notification</span></span>|<span data-ttu-id="978a0-115">1</span><span class="sxs-lookup"><span data-stu-id="978a0-115">1</span></span>|<span data-ttu-id="978a0-116">发送通知</span><span class="sxs-lookup"><span data-stu-id="978a0-116">Send Notification</span></span>|
|<span data-ttu-id="978a0-117">block</span><span class="sxs-lookup"><span data-stu-id="978a0-117">block</span></span>|<span data-ttu-id="978a0-118">2</span><span class="sxs-lookup"><span data-stu-id="978a0-118">2</span></span>|<span data-ttu-id="978a0-119">在 AAD 中阻止设备</span><span class="sxs-lookup"><span data-stu-id="978a0-119">Block the device in AAD</span></span>|
|<span data-ttu-id="978a0-120">retire</span><span class="sxs-lookup"><span data-stu-id="978a0-120">retire</span></span>|<span data-ttu-id="978a0-121">3</span><span class="sxs-lookup"><span data-stu-id="978a0-121">3</span></span>|<span data-ttu-id="978a0-122">停用设备</span><span class="sxs-lookup"><span data-stu-id="978a0-122">Retire the device</span></span>|
|<span data-ttu-id="978a0-123">wipe</span><span class="sxs-lookup"><span data-stu-id="978a0-123">wipe</span></span>|<span data-ttu-id="978a0-124">4 </span><span class="sxs-lookup"><span data-stu-id="978a0-124">4</span></span>|<span data-ttu-id="978a0-125">擦除设备</span><span class="sxs-lookup"><span data-stu-id="978a0-125">Wipe the device</span></span>|
|<span data-ttu-id="978a0-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="978a0-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="978a0-127">5 </span><span class="sxs-lookup"><span data-stu-id="978a0-127">5</span></span>|<span data-ttu-id="978a0-128">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="978a0-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="978a0-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="978a0-129">pushNotification</span></span>|<span data-ttu-id="978a0-130">9 </span><span class="sxs-lookup"><span data-stu-id="978a0-130">9</span></span>|<span data-ttu-id="978a0-131">向设备发送推送通知</span><span class="sxs-lookup"><span data-stu-id="978a0-131">Send push notification to device</span></span>|




