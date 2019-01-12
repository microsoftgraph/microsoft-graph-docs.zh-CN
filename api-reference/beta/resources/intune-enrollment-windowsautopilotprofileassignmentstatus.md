---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1427ffeb45862312d92fdf02a00a242725894d36
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962630"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="e67ae-103">windowsAutopilotProfileAssignmentStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e67ae-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="e67ae-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e67ae-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e67ae-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e67ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e67ae-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e67ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e67ae-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e67ae-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="e67ae-108">成员</span><span class="sxs-lookup"><span data-stu-id="e67ae-108">Members</span></span>
|<span data-ttu-id="e67ae-109">成员</span><span class="sxs-lookup"><span data-stu-id="e67ae-109">Member</span></span>|<span data-ttu-id="e67ae-110">值</span><span class="sxs-lookup"><span data-stu-id="e67ae-110">Value</span></span>|<span data-ttu-id="e67ae-111">说明</span><span class="sxs-lookup"><span data-stu-id="e67ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e67ae-112">unknown</span><span class="sxs-lookup"><span data-stu-id="e67ae-112">unknown</span></span>|<span data-ttu-id="e67ae-113">0</span><span class="sxs-lookup"><span data-stu-id="e67ae-113">0</span></span>|<span data-ttu-id="e67ae-114">未知的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="e67ae-114">Unknown assignment status</span></span>|
|<span data-ttu-id="e67ae-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="e67ae-115">assignedInSync</span></span>|<span data-ttu-id="e67ae-116">1</span><span class="sxs-lookup"><span data-stu-id="e67ae-116">1</span></span>|<span data-ttu-id="e67ae-117">分配 Intune 中成功的 Windows 自动试用计划同步</span><span class="sxs-lookup"><span data-stu-id="e67ae-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e67ae-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="e67ae-118">assignedOutOfSync</span></span>|<span data-ttu-id="e67ae-119">2</span><span class="sxs-lookup"><span data-stu-id="e67ae-119">2</span></span>|<span data-ttu-id="e67ae-120">分配 Intune 中成功的不与同步 Windows 自动试用计划</span><span class="sxs-lookup"><span data-stu-id="e67ae-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e67ae-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="e67ae-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="e67ae-122">3</span><span class="sxs-lookup"><span data-stu-id="e67ae-122">3</span></span>|<span data-ttu-id="e67ae-123">Intune 和任一中同步中成功分配或与 Windows 自动试用计划不同步</span><span class="sxs-lookup"><span data-stu-id="e67ae-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e67ae-124">notAssigned</span><span class="sxs-lookup"><span data-stu-id="e67ae-124">notAssigned</span></span>|<span data-ttu-id="e67ae-125">4</span><span class="sxs-lookup"><span data-stu-id="e67ae-125">4</span></span>|<span data-ttu-id="e67ae-126">未分配</span><span class="sxs-lookup"><span data-stu-id="e67ae-126">Not assigned</span></span>|
|<span data-ttu-id="e67ae-127">挂起</span><span class="sxs-lookup"><span data-stu-id="e67ae-127">pending</span></span>|<span data-ttu-id="e67ae-128">5</span><span class="sxs-lookup"><span data-stu-id="e67ae-128">5</span></span>|<span data-ttu-id="e67ae-129">待处理的工作分配</span><span class="sxs-lookup"><span data-stu-id="e67ae-129">Pending assignment</span></span>|
|<span data-ttu-id="e67ae-130">failed</span><span class="sxs-lookup"><span data-stu-id="e67ae-130">failed</span></span>|<span data-ttu-id="e67ae-131">6</span><span class="sxs-lookup"><span data-stu-id="e67ae-131">6</span></span>| <span data-ttu-id="e67ae-132">工作分配失败</span><span class="sxs-lookup"><span data-stu-id="e67ae-132">Assignment failed</span></span>|





