---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 91dfea5c94f634a367e6498edb9fc43ff733895b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528242"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="75703-103">windowsAutopilotProfileAssignmentStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="75703-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

<span data-ttu-id="75703-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="75703-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75703-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="75703-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75703-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="75703-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75703-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="75703-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="75703-108">成员</span><span class="sxs-lookup"><span data-stu-id="75703-108">Members</span></span>
|<span data-ttu-id="75703-109">成员</span><span class="sxs-lookup"><span data-stu-id="75703-109">Member</span></span>|<span data-ttu-id="75703-110">值</span><span class="sxs-lookup"><span data-stu-id="75703-110">Value</span></span>|<span data-ttu-id="75703-111">说明</span><span class="sxs-lookup"><span data-stu-id="75703-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75703-112">unknown</span><span class="sxs-lookup"><span data-stu-id="75703-112">unknown</span></span>|<span data-ttu-id="75703-113">0</span><span class="sxs-lookup"><span data-stu-id="75703-113">0</span></span>|<span data-ttu-id="75703-114">未知的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="75703-114">Unknown assignment status</span></span>|
|<span data-ttu-id="75703-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="75703-115">assignedInSync</span></span>|<span data-ttu-id="75703-116">1 </span><span class="sxs-lookup"><span data-stu-id="75703-116">1</span></span>|<span data-ttu-id="75703-117">在 Intune 中成功分配，并与 Windows 自动试用程序同步</span><span class="sxs-lookup"><span data-stu-id="75703-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="75703-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="75703-118">assignedOutOfSync</span></span>|<span data-ttu-id="75703-119">2 </span><span class="sxs-lookup"><span data-stu-id="75703-119">2</span></span>|<span data-ttu-id="75703-120">已在 Intune 中成功分配，与 Windows 自动试用程序不同步</span><span class="sxs-lookup"><span data-stu-id="75703-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="75703-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="75703-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="75703-122">3 </span><span class="sxs-lookup"><span data-stu-id="75703-122">3</span></span>|<span data-ttu-id="75703-123">在 Intune 中成功分配，并与 Windows 自动试用程序同步或不同步</span><span class="sxs-lookup"><span data-stu-id="75703-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="75703-124">notAssigned</span><span class="sxs-lookup"><span data-stu-id="75703-124">notAssigned</span></span>|<span data-ttu-id="75703-125">4 </span><span class="sxs-lookup"><span data-stu-id="75703-125">4</span></span>|<span data-ttu-id="75703-126">未分配</span><span class="sxs-lookup"><span data-stu-id="75703-126">Not assigned</span></span>|
|<span data-ttu-id="75703-127">决</span><span class="sxs-lookup"><span data-stu-id="75703-127">pending</span></span>|<span data-ttu-id="75703-128">5 </span><span class="sxs-lookup"><span data-stu-id="75703-128">5</span></span>|<span data-ttu-id="75703-129">挂起分配</span><span class="sxs-lookup"><span data-stu-id="75703-129">Pending assignment</span></span>|
|<span data-ttu-id="75703-130">未能</span><span class="sxs-lookup"><span data-stu-id="75703-130">failed</span></span>|<span data-ttu-id="75703-131">6 </span><span class="sxs-lookup"><span data-stu-id="75703-131">6</span></span>| <span data-ttu-id="75703-132">分配失败</span><span class="sxs-lookup"><span data-stu-id="75703-132">Assignment failed</span></span>|



