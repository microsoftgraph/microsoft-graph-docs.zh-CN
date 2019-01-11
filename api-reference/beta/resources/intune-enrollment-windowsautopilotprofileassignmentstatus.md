---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 48d08ad4d4c80c3d5a68cca5af36c958deaac819
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869641"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="e1787-103">windowsAutopilotProfileAssignmentStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e1787-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="e1787-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e1787-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1787-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e1787-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1787-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e1787-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1787-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e1787-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="e1787-108">成员</span><span class="sxs-lookup"><span data-stu-id="e1787-108">Members</span></span>
|<span data-ttu-id="e1787-109">成员</span><span class="sxs-lookup"><span data-stu-id="e1787-109">Member</span></span>|<span data-ttu-id="e1787-110">值</span><span class="sxs-lookup"><span data-stu-id="e1787-110">Value</span></span>|<span data-ttu-id="e1787-111">Description</span><span class="sxs-lookup"><span data-stu-id="e1787-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1787-112">unknown</span><span class="sxs-lookup"><span data-stu-id="e1787-112">unknown</span></span>|<span data-ttu-id="e1787-113">0</span><span class="sxs-lookup"><span data-stu-id="e1787-113">0</span></span>|<span data-ttu-id="e1787-114">未知的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="e1787-114">Unknown assignment status</span></span>|
|<span data-ttu-id="e1787-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="e1787-115">assignedInSync</span></span>|<span data-ttu-id="e1787-116">1</span><span class="sxs-lookup"><span data-stu-id="e1787-116">1</span></span>|<span data-ttu-id="e1787-117">分配 Intune 中成功的 Windows 自动试用计划同步</span><span class="sxs-lookup"><span data-stu-id="e1787-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e1787-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="e1787-118">assignedOutOfSync</span></span>|<span data-ttu-id="e1787-119">2</span><span class="sxs-lookup"><span data-stu-id="e1787-119">2</span></span>|<span data-ttu-id="e1787-120">分配 Intune 中成功的不与同步 Windows 自动试用计划</span><span class="sxs-lookup"><span data-stu-id="e1787-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e1787-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="e1787-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="e1787-122">3</span><span class="sxs-lookup"><span data-stu-id="e1787-122">3</span></span>|<span data-ttu-id="e1787-123">Intune 和任一中同步中成功分配或与 Windows 自动试用计划不同步</span><span class="sxs-lookup"><span data-stu-id="e1787-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e1787-124">notAssigned</span><span class="sxs-lookup"><span data-stu-id="e1787-124">notAssigned</span></span>|<span data-ttu-id="e1787-125">4</span><span class="sxs-lookup"><span data-stu-id="e1787-125">4</span></span>|<span data-ttu-id="e1787-126">未分配</span><span class="sxs-lookup"><span data-stu-id="e1787-126">Not assigned</span></span>|
|<span data-ttu-id="e1787-127">挂起</span><span class="sxs-lookup"><span data-stu-id="e1787-127">pending</span></span>|<span data-ttu-id="e1787-128">5</span><span class="sxs-lookup"><span data-stu-id="e1787-128">5</span></span>|<span data-ttu-id="e1787-129">待处理的工作分配</span><span class="sxs-lookup"><span data-stu-id="e1787-129">Pending assignment</span></span>|
|<span data-ttu-id="e1787-130">failed</span><span class="sxs-lookup"><span data-stu-id="e1787-130">failed</span></span>|<span data-ttu-id="e1787-131">6</span><span class="sxs-lookup"><span data-stu-id="e1787-131">6</span></span>| <span data-ttu-id="e1787-132">工作分配失败</span><span class="sxs-lookup"><span data-stu-id="e1787-132">Assignment failed</span></span>|





