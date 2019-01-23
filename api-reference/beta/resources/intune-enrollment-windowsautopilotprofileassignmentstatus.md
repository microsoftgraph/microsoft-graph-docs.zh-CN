---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68612e2f4ccee46612c82237630efafda484b7e9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419119"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="51ff7-103">windowsAutopilotProfileAssignmentStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="51ff7-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="51ff7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="51ff7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="51ff7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="51ff7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51ff7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51ff7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51ff7-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="51ff7-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="51ff7-108">成员</span><span class="sxs-lookup"><span data-stu-id="51ff7-108">Members</span></span>
|<span data-ttu-id="51ff7-109">成员</span><span class="sxs-lookup"><span data-stu-id="51ff7-109">Member</span></span>|<span data-ttu-id="51ff7-110">值</span><span class="sxs-lookup"><span data-stu-id="51ff7-110">Value</span></span>|<span data-ttu-id="51ff7-111">说明</span><span class="sxs-lookup"><span data-stu-id="51ff7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ff7-112">unknown</span><span class="sxs-lookup"><span data-stu-id="51ff7-112">unknown</span></span>|<span data-ttu-id="51ff7-113">0</span><span class="sxs-lookup"><span data-stu-id="51ff7-113">0</span></span>|<span data-ttu-id="51ff7-114">未知的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="51ff7-114">Unknown assignment status</span></span>|
|<span data-ttu-id="51ff7-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="51ff7-115">assignedInSync</span></span>|<span data-ttu-id="51ff7-116">1</span><span class="sxs-lookup"><span data-stu-id="51ff7-116">1</span></span>|<span data-ttu-id="51ff7-117">分配 Intune 中成功的 Windows 自动试用计划同步</span><span class="sxs-lookup"><span data-stu-id="51ff7-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="51ff7-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="51ff7-118">assignedOutOfSync</span></span>|<span data-ttu-id="51ff7-119">2</span><span class="sxs-lookup"><span data-stu-id="51ff7-119">2</span></span>|<span data-ttu-id="51ff7-120">分配 Intune 中成功的不与同步 Windows 自动试用计划</span><span class="sxs-lookup"><span data-stu-id="51ff7-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="51ff7-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="51ff7-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="51ff7-122">3</span><span class="sxs-lookup"><span data-stu-id="51ff7-122">3</span></span>|<span data-ttu-id="51ff7-123">Intune 和任一中同步中成功分配或与 Windows 自动试用计划不同步</span><span class="sxs-lookup"><span data-stu-id="51ff7-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="51ff7-124">notAssigned</span><span class="sxs-lookup"><span data-stu-id="51ff7-124">notAssigned</span></span>|<span data-ttu-id="51ff7-125">4</span><span class="sxs-lookup"><span data-stu-id="51ff7-125">4</span></span>|<span data-ttu-id="51ff7-126">未分配</span><span class="sxs-lookup"><span data-stu-id="51ff7-126">Not assigned</span></span>|
|<span data-ttu-id="51ff7-127">挂起</span><span class="sxs-lookup"><span data-stu-id="51ff7-127">pending</span></span>|<span data-ttu-id="51ff7-128">5</span><span class="sxs-lookup"><span data-stu-id="51ff7-128">5</span></span>|<span data-ttu-id="51ff7-129">待处理的工作分配</span><span class="sxs-lookup"><span data-stu-id="51ff7-129">Pending assignment</span></span>|
|<span data-ttu-id="51ff7-130">failed</span><span class="sxs-lookup"><span data-stu-id="51ff7-130">failed</span></span>|<span data-ttu-id="51ff7-131">6</span><span class="sxs-lookup"><span data-stu-id="51ff7-131">6</span></span>| <span data-ttu-id="51ff7-132">工作分配失败</span><span class="sxs-lookup"><span data-stu-id="51ff7-132">Assignment failed</span></span>|




