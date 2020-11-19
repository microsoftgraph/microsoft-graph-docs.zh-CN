---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a6ac21decb96434d7392e0d647ad4e9c2e07621f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288647"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="d849c-103">windowsAutopilotProfileAssignmentStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d849c-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

<span data-ttu-id="d849c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d849c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d849c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d849c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d849c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d849c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d849c-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d849c-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="d849c-108">成员</span><span class="sxs-lookup"><span data-stu-id="d849c-108">Members</span></span>
|<span data-ttu-id="d849c-109">成员</span><span class="sxs-lookup"><span data-stu-id="d849c-109">Member</span></span>|<span data-ttu-id="d849c-110">值</span><span class="sxs-lookup"><span data-stu-id="d849c-110">Value</span></span>|<span data-ttu-id="d849c-111">Description</span><span class="sxs-lookup"><span data-stu-id="d849c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d849c-112">unknown</span><span class="sxs-lookup"><span data-stu-id="d849c-112">unknown</span></span>|<span data-ttu-id="d849c-113">0</span><span class="sxs-lookup"><span data-stu-id="d849c-113">0</span></span>|<span data-ttu-id="d849c-114">未知的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="d849c-114">Unknown assignment status</span></span>|
|<span data-ttu-id="d849c-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="d849c-115">assignedInSync</span></span>|<span data-ttu-id="d849c-116">1</span><span class="sxs-lookup"><span data-stu-id="d849c-116">1</span></span>|<span data-ttu-id="d849c-117">在 Intune 中成功分配，并与 Windows 自动试用程序同步</span><span class="sxs-lookup"><span data-stu-id="d849c-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="d849c-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="d849c-118">assignedOutOfSync</span></span>|<span data-ttu-id="d849c-119">双面</span><span class="sxs-lookup"><span data-stu-id="d849c-119">2</span></span>|<span data-ttu-id="d849c-120">已在 Intune 中成功分配，与 Windows 自动试用程序不同步</span><span class="sxs-lookup"><span data-stu-id="d849c-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="d849c-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="d849c-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="d849c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="d849c-122">3</span></span>|<span data-ttu-id="d849c-123">在 Intune 中成功分配，并与 Windows 自动试用程序同步或不同步</span><span class="sxs-lookup"><span data-stu-id="d849c-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="d849c-124">notAssigned</span><span class="sxs-lookup"><span data-stu-id="d849c-124">notAssigned</span></span>|<span data-ttu-id="d849c-125">4 </span><span class="sxs-lookup"><span data-stu-id="d849c-125">4</span></span>|<span data-ttu-id="d849c-126">未分配</span><span class="sxs-lookup"><span data-stu-id="d849c-126">Not assigned</span></span>|
|<span data-ttu-id="d849c-127">决</span><span class="sxs-lookup"><span data-stu-id="d849c-127">pending</span></span>|<span data-ttu-id="d849c-128">5 </span><span class="sxs-lookup"><span data-stu-id="d849c-128">5</span></span>|<span data-ttu-id="d849c-129">挂起分配</span><span class="sxs-lookup"><span data-stu-id="d849c-129">Pending assignment</span></span>|
|<span data-ttu-id="d849c-130">未能</span><span class="sxs-lookup"><span data-stu-id="d849c-130">failed</span></span>|<span data-ttu-id="d849c-131">6 </span><span class="sxs-lookup"><span data-stu-id="d849c-131">6</span></span>| <span data-ttu-id="d849c-132">分配失败</span><span class="sxs-lookup"><span data-stu-id="d849c-132">Assignment failed</span></span>|




