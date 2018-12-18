---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: tfitzmac
ms.openlocfilehash: 84bef94d7352c13b49f223b859cea218932f8cad
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328684"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="a7659-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a7659-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="a7659-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a7659-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7659-105">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="a7659-105">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="a7659-106">成员</span><span class="sxs-lookup"><span data-stu-id="a7659-106">Members</span></span>
|<span data-ttu-id="a7659-107">成员</span><span class="sxs-lookup"><span data-stu-id="a7659-107">Member</span></span>|<span data-ttu-id="a7659-108">值</span><span class="sxs-lookup"><span data-stu-id="a7659-108">Value</span></span>|<span data-ttu-id="a7659-109">说明</span><span class="sxs-lookup"><span data-stu-id="a7659-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7659-110">noAction</span><span class="sxs-lookup"><span data-stu-id="a7659-110">noAction</span></span>|<span data-ttu-id="a7659-111">0</span><span class="sxs-lookup"><span data-stu-id="a7659-111">0</span></span>|<span data-ttu-id="a7659-112">任何操作</span><span class="sxs-lookup"><span data-stu-id="a7659-112">No Action</span></span>|
|<span data-ttu-id="a7659-113">通知</span><span class="sxs-lookup"><span data-stu-id="a7659-113">notification</span></span>|<span data-ttu-id="a7659-114">1</span><span class="sxs-lookup"><span data-stu-id="a7659-114">1</span></span>|<span data-ttu-id="a7659-115">发送通知</span><span class="sxs-lookup"><span data-stu-id="a7659-115">Send Notification</span></span>|
|<span data-ttu-id="a7659-116">阻止</span><span class="sxs-lookup"><span data-stu-id="a7659-116">block</span></span>|<span data-ttu-id="a7659-117">2</span><span class="sxs-lookup"><span data-stu-id="a7659-117">2</span></span>|<span data-ttu-id="a7659-118">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="a7659-118">Block the device in AAD</span></span>|
|<span data-ttu-id="a7659-119">停用</span><span class="sxs-lookup"><span data-stu-id="a7659-119">retire</span></span>|<span data-ttu-id="a7659-120">3</span><span class="sxs-lookup"><span data-stu-id="a7659-120">3</span></span>|<span data-ttu-id="a7659-121">停用设备</span><span class="sxs-lookup"><span data-stu-id="a7659-121">Retire the device</span></span>|
|<span data-ttu-id="a7659-122">擦除</span><span class="sxs-lookup"><span data-stu-id="a7659-122">wipe</span></span>|<span data-ttu-id="a7659-123">4</span><span class="sxs-lookup"><span data-stu-id="a7659-123">4</span></span>|<span data-ttu-id="a7659-124">擦除设备</span><span class="sxs-lookup"><span data-stu-id="a7659-124">Wipe the device</span></span>|
|<span data-ttu-id="a7659-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="a7659-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="a7659-126">5</span><span class="sxs-lookup"><span data-stu-id="a7659-126">5</span></span>|<span data-ttu-id="a7659-127">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="a7659-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="a7659-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="a7659-128">pushNotification</span></span>|<span data-ttu-id="a7659-129">9</span><span class="sxs-lookup"><span data-stu-id="a7659-129">9</span></span>|<span data-ttu-id="a7659-130">向设备发送推送通知</span><span class="sxs-lookup"><span data-stu-id="a7659-130">Send push notification to device</span></span>|



