---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b729386eeb76197ed426163d1882afc6aec836a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359654"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="89fb5-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="89fb5-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="89fb5-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89fb5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89fb5-105">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="89fb5-105">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="89fb5-106">成员</span><span class="sxs-lookup"><span data-stu-id="89fb5-106">Members</span></span>
|<span data-ttu-id="89fb5-107">成员</span><span class="sxs-lookup"><span data-stu-id="89fb5-107">Member</span></span>|<span data-ttu-id="89fb5-108">值</span><span class="sxs-lookup"><span data-stu-id="89fb5-108">Value</span></span>|<span data-ttu-id="89fb5-109">说明</span><span class="sxs-lookup"><span data-stu-id="89fb5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89fb5-110">noAction</span><span class="sxs-lookup"><span data-stu-id="89fb5-110">noAction</span></span>|<span data-ttu-id="89fb5-111">0</span><span class="sxs-lookup"><span data-stu-id="89fb5-111">0</span></span>|<span data-ttu-id="89fb5-112">无操作</span><span class="sxs-lookup"><span data-stu-id="89fb5-112">No Action</span></span>|
|<span data-ttu-id="89fb5-113">通告</span><span class="sxs-lookup"><span data-stu-id="89fb5-113">notification</span></span>|<span data-ttu-id="89fb5-114">1</span><span class="sxs-lookup"><span data-stu-id="89fb5-114">1</span></span>|<span data-ttu-id="89fb5-115">发送通知</span><span class="sxs-lookup"><span data-stu-id="89fb5-115">Send Notification</span></span>|
|<span data-ttu-id="89fb5-116">数据</span><span class="sxs-lookup"><span data-stu-id="89fb5-116">block</span></span>|<span data-ttu-id="89fb5-117">双面</span><span class="sxs-lookup"><span data-stu-id="89fb5-117">2</span></span>|<span data-ttu-id="89fb5-118">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="89fb5-118">Block the device in AAD</span></span>|
|<span data-ttu-id="89fb5-119">注销</span><span class="sxs-lookup"><span data-stu-id="89fb5-119">retire</span></span>|<span data-ttu-id="89fb5-120">第三章</span><span class="sxs-lookup"><span data-stu-id="89fb5-120">3</span></span>|<span data-ttu-id="89fb5-121">停用设备</span><span class="sxs-lookup"><span data-stu-id="89fb5-121">Retire the device</span></span>|
|<span data-ttu-id="89fb5-122">擦</span><span class="sxs-lookup"><span data-stu-id="89fb5-122">wipe</span></span>|<span data-ttu-id="89fb5-123">4</span><span class="sxs-lookup"><span data-stu-id="89fb5-123">4</span></span>|<span data-ttu-id="89fb5-124">擦除设备</span><span class="sxs-lookup"><span data-stu-id="89fb5-124">Wipe the device</span></span>|
|<span data-ttu-id="89fb5-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="89fb5-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="89fb5-126">5</span><span class="sxs-lookup"><span data-stu-id="89fb5-126">5</span></span>|<span data-ttu-id="89fb5-127">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="89fb5-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="89fb5-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="89fb5-128">pushNotification</span></span>|<span data-ttu-id="89fb5-129">第</span><span class="sxs-lookup"><span data-stu-id="89fb5-129">9</span></span>|<span data-ttu-id="89fb5-130">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="89fb5-130">Send push notification to device</span></span>|




