---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7100e5881049900bb474e20060ac916ec1199a29
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783366"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="718af-103">windowsAutopilotProfileAssignmentStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="718af-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="718af-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="718af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="718af-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="718af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="718af-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="718af-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="718af-107">成员</span><span class="sxs-lookup"><span data-stu-id="718af-107">Members</span></span>
|<span data-ttu-id="718af-108">成员</span><span class="sxs-lookup"><span data-stu-id="718af-108">Member</span></span>|<span data-ttu-id="718af-109">值</span><span class="sxs-lookup"><span data-stu-id="718af-109">Value</span></span>|<span data-ttu-id="718af-110">说明</span><span class="sxs-lookup"><span data-stu-id="718af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="718af-111">unknown</span><span class="sxs-lookup"><span data-stu-id="718af-111">unknown</span></span>|<span data-ttu-id="718af-112">0</span><span class="sxs-lookup"><span data-stu-id="718af-112">0</span></span>|<span data-ttu-id="718af-113">未知的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="718af-113">Unknown assignment status</span></span>|
|<span data-ttu-id="718af-114">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="718af-114">assignedInSync</span></span>|<span data-ttu-id="718af-115">1</span><span class="sxs-lookup"><span data-stu-id="718af-115">1</span></span>|<span data-ttu-id="718af-116">在 Intune 中成功分配，并与 Windows 自动试用程序同步</span><span class="sxs-lookup"><span data-stu-id="718af-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="718af-117">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="718af-117">assignedOutOfSync</span></span>|<span data-ttu-id="718af-118">双面</span><span class="sxs-lookup"><span data-stu-id="718af-118">2</span></span>|<span data-ttu-id="718af-119">已在 Intune 中成功分配，与 Windows 自动试用程序不同步</span><span class="sxs-lookup"><span data-stu-id="718af-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="718af-120">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="718af-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="718af-121">第三章</span><span class="sxs-lookup"><span data-stu-id="718af-121">3</span></span>|<span data-ttu-id="718af-122">在 Intune 中成功分配，并与 Windows 自动试用程序同步或不同步</span><span class="sxs-lookup"><span data-stu-id="718af-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="718af-123">notAssigned</span><span class="sxs-lookup"><span data-stu-id="718af-123">notAssigned</span></span>|<span data-ttu-id="718af-124">4 </span><span class="sxs-lookup"><span data-stu-id="718af-124">4</span></span>|<span data-ttu-id="718af-125">未分配</span><span class="sxs-lookup"><span data-stu-id="718af-125">Not assigned</span></span>|
|<span data-ttu-id="718af-126">决</span><span class="sxs-lookup"><span data-stu-id="718af-126">pending</span></span>|<span data-ttu-id="718af-127">5 </span><span class="sxs-lookup"><span data-stu-id="718af-127">5</span></span>|<span data-ttu-id="718af-128">挂起分配</span><span class="sxs-lookup"><span data-stu-id="718af-128">Pending assignment</span></span>|
|<span data-ttu-id="718af-129">未能</span><span class="sxs-lookup"><span data-stu-id="718af-129">failed</span></span>|<span data-ttu-id="718af-130">6 </span><span class="sxs-lookup"><span data-stu-id="718af-130">6</span></span>| <span data-ttu-id="718af-131">分配失败</span><span class="sxs-lookup"><span data-stu-id="718af-131">Assignment failed</span></span>|



