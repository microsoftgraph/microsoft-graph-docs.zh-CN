---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ce8fe0a165d46e9dd59ac88759093e12b60d2028
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031576"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="24616-103">windowsAutopilotProfileAssignmentStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="24616-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

<span data-ttu-id="24616-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24616-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24616-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24616-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24616-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24616-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24616-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24616-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="24616-108">成员</span><span class="sxs-lookup"><span data-stu-id="24616-108">Members</span></span>
|<span data-ttu-id="24616-109">成员</span><span class="sxs-lookup"><span data-stu-id="24616-109">Member</span></span>|<span data-ttu-id="24616-110">值</span><span class="sxs-lookup"><span data-stu-id="24616-110">Value</span></span>|<span data-ttu-id="24616-111">说明</span><span class="sxs-lookup"><span data-stu-id="24616-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24616-112">unknown</span><span class="sxs-lookup"><span data-stu-id="24616-112">unknown</span></span>|<span data-ttu-id="24616-113">0</span><span class="sxs-lookup"><span data-stu-id="24616-113">0</span></span>|<span data-ttu-id="24616-114">未知的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="24616-114">Unknown assignment status</span></span>|
|<span data-ttu-id="24616-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="24616-115">assignedInSync</span></span>|<span data-ttu-id="24616-116">1 </span><span class="sxs-lookup"><span data-stu-id="24616-116">1</span></span>|<span data-ttu-id="24616-117">在 Intune 中成功分配，并与 Windows 自动试用程序同步</span><span class="sxs-lookup"><span data-stu-id="24616-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="24616-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="24616-118">assignedOutOfSync</span></span>|<span data-ttu-id="24616-119">2 </span><span class="sxs-lookup"><span data-stu-id="24616-119">2</span></span>|<span data-ttu-id="24616-120">已在 Intune 中成功分配，与 Windows 自动试用程序不同步</span><span class="sxs-lookup"><span data-stu-id="24616-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="24616-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="24616-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="24616-122">第三章</span><span class="sxs-lookup"><span data-stu-id="24616-122">3</span></span>|<span data-ttu-id="24616-123">在 Intune 中成功分配，并与 Windows 自动试用程序同步或不同步</span><span class="sxs-lookup"><span data-stu-id="24616-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="24616-124">notAssigned</span><span class="sxs-lookup"><span data-stu-id="24616-124">notAssigned</span></span>|<span data-ttu-id="24616-125">4 </span><span class="sxs-lookup"><span data-stu-id="24616-125">4</span></span>|<span data-ttu-id="24616-126">未分配</span><span class="sxs-lookup"><span data-stu-id="24616-126">Not assigned</span></span>|
|<span data-ttu-id="24616-127">决</span><span class="sxs-lookup"><span data-stu-id="24616-127">pending</span></span>|<span data-ttu-id="24616-128">5 </span><span class="sxs-lookup"><span data-stu-id="24616-128">5</span></span>|<span data-ttu-id="24616-129">挂起分配</span><span class="sxs-lookup"><span data-stu-id="24616-129">Pending assignment</span></span>|
|<span data-ttu-id="24616-130">未能</span><span class="sxs-lookup"><span data-stu-id="24616-130">failed</span></span>|<span data-ttu-id="24616-131">6 </span><span class="sxs-lookup"><span data-stu-id="24616-131">6</span></span>| <span data-ttu-id="24616-132">分配失败</span><span class="sxs-lookup"><span data-stu-id="24616-132">Assignment failed</span></span>|






