---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3be930f3289891235a1462d0322323eb9b44bf60
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989747"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="1d761-103">windowsAutopilotProfileAssignmentStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1d761-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="1d761-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d761-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d761-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d761-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d761-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1d761-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="1d761-107">成员</span><span class="sxs-lookup"><span data-stu-id="1d761-107">Members</span></span>
|<span data-ttu-id="1d761-108">成员</span><span class="sxs-lookup"><span data-stu-id="1d761-108">Member</span></span>|<span data-ttu-id="1d761-109">值</span><span class="sxs-lookup"><span data-stu-id="1d761-109">Value</span></span>|<span data-ttu-id="1d761-110">说明</span><span class="sxs-lookup"><span data-stu-id="1d761-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d761-111">unknown</span><span class="sxs-lookup"><span data-stu-id="1d761-111">unknown</span></span>|<span data-ttu-id="1d761-112">0</span><span class="sxs-lookup"><span data-stu-id="1d761-112">0</span></span>|<span data-ttu-id="1d761-113">未知的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="1d761-113">Unknown assignment status</span></span>|
|<span data-ttu-id="1d761-114">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="1d761-114">assignedInSync</span></span>|<span data-ttu-id="1d761-115">1</span><span class="sxs-lookup"><span data-stu-id="1d761-115">1</span></span>|<span data-ttu-id="1d761-116">在 Intune 中成功分配, 并与 Windows 自动试用程序同步</span><span class="sxs-lookup"><span data-stu-id="1d761-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="1d761-117">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="1d761-117">assignedOutOfSync</span></span>|<span data-ttu-id="1d761-118">双面</span><span class="sxs-lookup"><span data-stu-id="1d761-118">2</span></span>|<span data-ttu-id="1d761-119">已在 Intune 中成功分配, 与 Windows 自动试用程序不同步</span><span class="sxs-lookup"><span data-stu-id="1d761-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="1d761-120">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="1d761-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="1d761-121">第三章</span><span class="sxs-lookup"><span data-stu-id="1d761-121">3</span></span>|<span data-ttu-id="1d761-122">在 Intune 中成功分配, 并与 Windows 自动试用程序同步或不同步</span><span class="sxs-lookup"><span data-stu-id="1d761-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="1d761-123">notAssigned</span><span class="sxs-lookup"><span data-stu-id="1d761-123">notAssigned</span></span>|<span data-ttu-id="1d761-124">4</span><span class="sxs-lookup"><span data-stu-id="1d761-124">4</span></span>|<span data-ttu-id="1d761-125">未分配</span><span class="sxs-lookup"><span data-stu-id="1d761-125">Not assigned</span></span>|
|<span data-ttu-id="1d761-126">决</span><span class="sxs-lookup"><span data-stu-id="1d761-126">pending</span></span>|<span data-ttu-id="1d761-127">5</span><span class="sxs-lookup"><span data-stu-id="1d761-127">5</span></span>|<span data-ttu-id="1d761-128">挂起分配</span><span class="sxs-lookup"><span data-stu-id="1d761-128">Pending assignment</span></span>|
|<span data-ttu-id="1d761-129">未能</span><span class="sxs-lookup"><span data-stu-id="1d761-129">failed</span></span>|<span data-ttu-id="1d761-130">型</span><span class="sxs-lookup"><span data-stu-id="1d761-130">6</span></span>| <span data-ttu-id="1d761-131">分配失败</span><span class="sxs-lookup"><span data-stu-id="1d761-131">Assignment failed</span></span>|





