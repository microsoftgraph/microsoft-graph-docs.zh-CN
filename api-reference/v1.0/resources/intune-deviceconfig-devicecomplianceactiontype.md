---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
ms.openlocfilehash: e0ec7380dcf581d811057ff5bf87edbc376d70c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007624"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="10c75-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="10c75-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="10c75-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="10c75-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10c75-105">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="10c75-105">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="10c75-106">成员</span><span class="sxs-lookup"><span data-stu-id="10c75-106">Members</span></span>
|<span data-ttu-id="10c75-107">成员</span><span class="sxs-lookup"><span data-stu-id="10c75-107">Member</span></span>|<span data-ttu-id="10c75-108">值</span><span class="sxs-lookup"><span data-stu-id="10c75-108">Value</span></span>|<span data-ttu-id="10c75-109">说明</span><span class="sxs-lookup"><span data-stu-id="10c75-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10c75-110">noAction</span><span class="sxs-lookup"><span data-stu-id="10c75-110">noAction</span></span>|<span data-ttu-id="10c75-111">0</span><span class="sxs-lookup"><span data-stu-id="10c75-111">0</span></span>|<span data-ttu-id="10c75-112">任何操作</span><span class="sxs-lookup"><span data-stu-id="10c75-112">No Action</span></span>|
|<span data-ttu-id="10c75-113">通知</span><span class="sxs-lookup"><span data-stu-id="10c75-113">notification</span></span>|<span data-ttu-id="10c75-114">1</span><span class="sxs-lookup"><span data-stu-id="10c75-114">1</span></span>|<span data-ttu-id="10c75-115">发送通知</span><span class="sxs-lookup"><span data-stu-id="10c75-115">Send Notification</span></span>|
|<span data-ttu-id="10c75-116">阻止</span><span class="sxs-lookup"><span data-stu-id="10c75-116">block</span></span>|<span data-ttu-id="10c75-117">2</span><span class="sxs-lookup"><span data-stu-id="10c75-117">2</span></span>|<span data-ttu-id="10c75-118">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="10c75-118">Block the device in AAD</span></span>|
|<span data-ttu-id="10c75-119">停用</span><span class="sxs-lookup"><span data-stu-id="10c75-119">retire</span></span>|<span data-ttu-id="10c75-120">3</span><span class="sxs-lookup"><span data-stu-id="10c75-120">3</span></span>|<span data-ttu-id="10c75-121">停用设备</span><span class="sxs-lookup"><span data-stu-id="10c75-121">Retire the device</span></span>|
|<span data-ttu-id="10c75-122">擦除</span><span class="sxs-lookup"><span data-stu-id="10c75-122">wipe</span></span>|<span data-ttu-id="10c75-123">4</span><span class="sxs-lookup"><span data-stu-id="10c75-123">4</span></span>|<span data-ttu-id="10c75-124">擦除设备</span><span class="sxs-lookup"><span data-stu-id="10c75-124">Wipe the device</span></span>|
|<span data-ttu-id="10c75-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="10c75-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="10c75-126">5</span><span class="sxs-lookup"><span data-stu-id="10c75-126">5</span></span>|<span data-ttu-id="10c75-127">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="10c75-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="10c75-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="10c75-128">pushNotification</span></span>|<span data-ttu-id="10c75-129">9</span><span class="sxs-lookup"><span data-stu-id="10c75-129">9</span></span>|<span data-ttu-id="10c75-130">向设备发送推送通知</span><span class="sxs-lookup"><span data-stu-id="10c75-130">Send push notification to device</span></span>|



