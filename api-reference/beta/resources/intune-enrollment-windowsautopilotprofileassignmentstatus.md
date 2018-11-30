---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
ms.openlocfilehash: 0ec6dfaa6dbc87fe1d38a495ac177a84e70796a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041613"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="aa76d-103">windowsAutopilotProfileAssignmentStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="aa76d-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="aa76d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aa76d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa76d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa76d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa76d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aa76d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa76d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="aa76d-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="aa76d-108">成员</span><span class="sxs-lookup"><span data-stu-id="aa76d-108">Members</span></span>
|<span data-ttu-id="aa76d-109">成员</span><span class="sxs-lookup"><span data-stu-id="aa76d-109">Member</span></span>|<span data-ttu-id="aa76d-110">值</span><span class="sxs-lookup"><span data-stu-id="aa76d-110">Value</span></span>|<span data-ttu-id="aa76d-111">说明</span><span class="sxs-lookup"><span data-stu-id="aa76d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa76d-112">unknown</span><span class="sxs-lookup"><span data-stu-id="aa76d-112">unknown</span></span>|<span data-ttu-id="aa76d-113">0</span><span class="sxs-lookup"><span data-stu-id="aa76d-113">0</span></span>|<span data-ttu-id="aa76d-114">未知的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="aa76d-114">Unknown assignment status</span></span>|
|<span data-ttu-id="aa76d-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="aa76d-115">assignedInSync</span></span>|<span data-ttu-id="aa76d-116">1</span><span class="sxs-lookup"><span data-stu-id="aa76d-116">1</span></span>|<span data-ttu-id="aa76d-117">分配 Intune 中成功的 Windows 自动试用计划同步</span><span class="sxs-lookup"><span data-stu-id="aa76d-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="aa76d-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="aa76d-118">assignedOutOfSync</span></span>|<span data-ttu-id="aa76d-119">2</span><span class="sxs-lookup"><span data-stu-id="aa76d-119">2</span></span>|<span data-ttu-id="aa76d-120">分配 Intune 中成功的不与同步 Windows 自动试用计划</span><span class="sxs-lookup"><span data-stu-id="aa76d-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="aa76d-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="aa76d-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="aa76d-122">3</span><span class="sxs-lookup"><span data-stu-id="aa76d-122">3</span></span>|<span data-ttu-id="aa76d-123">Intune 和任一中同步中成功分配或与 Windows 自动试用计划不同步</span><span class="sxs-lookup"><span data-stu-id="aa76d-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="aa76d-124">notAssigned</span><span class="sxs-lookup"><span data-stu-id="aa76d-124">notAssigned</span></span>|<span data-ttu-id="aa76d-125">4</span><span class="sxs-lookup"><span data-stu-id="aa76d-125">4</span></span>|<span data-ttu-id="aa76d-126">未分配</span><span class="sxs-lookup"><span data-stu-id="aa76d-126">Not assigned</span></span>|
|<span data-ttu-id="aa76d-127">挂起</span><span class="sxs-lookup"><span data-stu-id="aa76d-127">pending</span></span>|<span data-ttu-id="aa76d-128">5</span><span class="sxs-lookup"><span data-stu-id="aa76d-128">5</span></span>|<span data-ttu-id="aa76d-129">待处理的工作分配</span><span class="sxs-lookup"><span data-stu-id="aa76d-129">Pending assignment</span></span>|
|<span data-ttu-id="aa76d-130">failed</span><span class="sxs-lookup"><span data-stu-id="aa76d-130">failed</span></span>|<span data-ttu-id="aa76d-131">6</span><span class="sxs-lookup"><span data-stu-id="aa76d-131">6</span></span>| <span data-ttu-id="aa76d-132">工作分配失败</span><span class="sxs-lookup"><span data-stu-id="aa76d-132">Assignment failed</span></span>|





