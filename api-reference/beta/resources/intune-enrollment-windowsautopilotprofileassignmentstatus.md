---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d7f946f113288ac95c87053a06ffd737de3dddc4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998995"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="99156-103">windowsAutopilotProfileAssignmentStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="99156-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="99156-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99156-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99156-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99156-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99156-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="99156-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="99156-107">成员</span><span class="sxs-lookup"><span data-stu-id="99156-107">Members</span></span>
|<span data-ttu-id="99156-108">成员</span><span class="sxs-lookup"><span data-stu-id="99156-108">Member</span></span>|<span data-ttu-id="99156-109">值</span><span class="sxs-lookup"><span data-stu-id="99156-109">Value</span></span>|<span data-ttu-id="99156-110">说明</span><span class="sxs-lookup"><span data-stu-id="99156-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99156-111">unknown</span><span class="sxs-lookup"><span data-stu-id="99156-111">unknown</span></span>|<span data-ttu-id="99156-112">0</span><span class="sxs-lookup"><span data-stu-id="99156-112">0</span></span>|<span data-ttu-id="99156-113">未知的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="99156-113">Unknown assignment status</span></span>|
|<span data-ttu-id="99156-114">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="99156-114">assignedInSync</span></span>|<span data-ttu-id="99156-115">1</span><span class="sxs-lookup"><span data-stu-id="99156-115">1</span></span>|<span data-ttu-id="99156-116">在 Intune 中成功分配, 并与 Windows 自动试用程序同步</span><span class="sxs-lookup"><span data-stu-id="99156-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="99156-117">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="99156-117">assignedOutOfSync</span></span>|<span data-ttu-id="99156-118">双面</span><span class="sxs-lookup"><span data-stu-id="99156-118">2</span></span>|<span data-ttu-id="99156-119">已在 Intune 中成功分配, 与 Windows 自动试用程序不同步</span><span class="sxs-lookup"><span data-stu-id="99156-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="99156-120">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="99156-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="99156-121">第三章</span><span class="sxs-lookup"><span data-stu-id="99156-121">3</span></span>|<span data-ttu-id="99156-122">在 Intune 中成功分配, 并与 Windows 自动试用程序同步或不同步</span><span class="sxs-lookup"><span data-stu-id="99156-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="99156-123">notAssigned</span><span class="sxs-lookup"><span data-stu-id="99156-123">notAssigned</span></span>|<span data-ttu-id="99156-124">4</span><span class="sxs-lookup"><span data-stu-id="99156-124">4</span></span>|<span data-ttu-id="99156-125">未分配</span><span class="sxs-lookup"><span data-stu-id="99156-125">Not assigned</span></span>|
|<span data-ttu-id="99156-126">决</span><span class="sxs-lookup"><span data-stu-id="99156-126">pending</span></span>|<span data-ttu-id="99156-127">5</span><span class="sxs-lookup"><span data-stu-id="99156-127">5</span></span>|<span data-ttu-id="99156-128">挂起分配</span><span class="sxs-lookup"><span data-stu-id="99156-128">Pending assignment</span></span>|
|<span data-ttu-id="99156-129">未能</span><span class="sxs-lookup"><span data-stu-id="99156-129">failed</span></span>|<span data-ttu-id="99156-130">型</span><span class="sxs-lookup"><span data-stu-id="99156-130">6</span></span>| <span data-ttu-id="99156-131">分配失败</span><span class="sxs-lookup"><span data-stu-id="99156-131">Assignment failed</span></span>|





