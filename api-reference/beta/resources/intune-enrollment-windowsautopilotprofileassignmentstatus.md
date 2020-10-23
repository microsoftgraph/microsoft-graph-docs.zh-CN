---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 93a956fa874fb50257da62fc9dbea59768e7a3cb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728905"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="1a7a7-103">windowsAutopilotProfileAssignmentStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1a7a7-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

<span data-ttu-id="1a7a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a7a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a7a7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a7a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a7a7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a7a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a7a7-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1a7a7-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="1a7a7-108">成员</span><span class="sxs-lookup"><span data-stu-id="1a7a7-108">Members</span></span>
|<span data-ttu-id="1a7a7-109">成员</span><span class="sxs-lookup"><span data-stu-id="1a7a7-109">Member</span></span>|<span data-ttu-id="1a7a7-110">值</span><span class="sxs-lookup"><span data-stu-id="1a7a7-110">Value</span></span>|<span data-ttu-id="1a7a7-111">说明</span><span class="sxs-lookup"><span data-stu-id="1a7a7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a7a7-112">unknown</span><span class="sxs-lookup"><span data-stu-id="1a7a7-112">unknown</span></span>|<span data-ttu-id="1a7a7-113">0</span><span class="sxs-lookup"><span data-stu-id="1a7a7-113">0</span></span>|<span data-ttu-id="1a7a7-114">未知的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="1a7a7-114">Unknown assignment status</span></span>|
|<span data-ttu-id="1a7a7-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="1a7a7-115">assignedInSync</span></span>|<span data-ttu-id="1a7a7-116">1</span><span class="sxs-lookup"><span data-stu-id="1a7a7-116">1</span></span>|<span data-ttu-id="1a7a7-117">在 Intune 中成功分配，并与 Windows 自动试用程序同步</span><span class="sxs-lookup"><span data-stu-id="1a7a7-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="1a7a7-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="1a7a7-118">assignedOutOfSync</span></span>|<span data-ttu-id="1a7a7-119">双面</span><span class="sxs-lookup"><span data-stu-id="1a7a7-119">2</span></span>|<span data-ttu-id="1a7a7-120">已在 Intune 中成功分配，与 Windows 自动试用程序不同步</span><span class="sxs-lookup"><span data-stu-id="1a7a7-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="1a7a7-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="1a7a7-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="1a7a7-122">第三章</span><span class="sxs-lookup"><span data-stu-id="1a7a7-122">3</span></span>|<span data-ttu-id="1a7a7-123">在 Intune 中成功分配，并与 Windows 自动试用程序同步或不同步</span><span class="sxs-lookup"><span data-stu-id="1a7a7-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="1a7a7-124">notAssigned</span><span class="sxs-lookup"><span data-stu-id="1a7a7-124">notAssigned</span></span>|<span data-ttu-id="1a7a7-125">4 </span><span class="sxs-lookup"><span data-stu-id="1a7a7-125">4</span></span>|<span data-ttu-id="1a7a7-126">未分配</span><span class="sxs-lookup"><span data-stu-id="1a7a7-126">Not assigned</span></span>|
|<span data-ttu-id="1a7a7-127">决</span><span class="sxs-lookup"><span data-stu-id="1a7a7-127">pending</span></span>|<span data-ttu-id="1a7a7-128">5 </span><span class="sxs-lookup"><span data-stu-id="1a7a7-128">5</span></span>|<span data-ttu-id="1a7a7-129">挂起分配</span><span class="sxs-lookup"><span data-stu-id="1a7a7-129">Pending assignment</span></span>|
|<span data-ttu-id="1a7a7-130">未能</span><span class="sxs-lookup"><span data-stu-id="1a7a7-130">failed</span></span>|<span data-ttu-id="1a7a7-131">6 </span><span class="sxs-lookup"><span data-stu-id="1a7a7-131">6</span></span>| <span data-ttu-id="1a7a7-132">分配失败</span><span class="sxs-lookup"><span data-stu-id="1a7a7-132">Assignment failed</span></span>|





