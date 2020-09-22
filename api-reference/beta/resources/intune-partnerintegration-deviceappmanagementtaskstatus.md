---
title: deviceAppManagementTaskStatus 枚举类型
description: 设备应用程序管理任务状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9d47b60bf805ba4f12345512c5d18b2c953c4467
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993663"
---
# <a name="deviceappmanagementtaskstatus-enum-type"></a><span data-ttu-id="5c641-103">deviceAppManagementTaskStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5c641-103">deviceAppManagementTaskStatus enum type</span></span>

<span data-ttu-id="5c641-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c641-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c641-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c641-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c641-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c641-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c641-107">设备应用程序管理任务状态。</span><span class="sxs-lookup"><span data-stu-id="5c641-107">Device app management task status.</span></span>

## <a name="members"></a><span data-ttu-id="5c641-108">成员</span><span class="sxs-lookup"><span data-stu-id="5c641-108">Members</span></span>
|<span data-ttu-id="5c641-109">成员</span><span class="sxs-lookup"><span data-stu-id="5c641-109">Member</span></span>|<span data-ttu-id="5c641-110">值</span><span class="sxs-lookup"><span data-stu-id="5c641-110">Value</span></span>|<span data-ttu-id="5c641-111">说明</span><span class="sxs-lookup"><span data-stu-id="5c641-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c641-112">unknown</span><span class="sxs-lookup"><span data-stu-id="5c641-112">unknown</span></span>|<span data-ttu-id="5c641-113">0</span><span class="sxs-lookup"><span data-stu-id="5c641-113">0</span></span>|<span data-ttu-id="5c641-114">状态未定义。</span><span class="sxs-lookup"><span data-stu-id="5c641-114">State is undefined.</span></span>|
|<span data-ttu-id="5c641-115">决</span><span class="sxs-lookup"><span data-stu-id="5c641-115">pending</span></span>|<span data-ttu-id="5c641-116">1 </span><span class="sxs-lookup"><span data-stu-id="5c641-116">1</span></span>|<span data-ttu-id="5c641-117">任务已准备好进行审阅。</span><span class="sxs-lookup"><span data-stu-id="5c641-117">The task is ready for review.</span></span>|
|<span data-ttu-id="5c641-118">工作</span><span class="sxs-lookup"><span data-stu-id="5c641-118">active</span></span>|<span data-ttu-id="5c641-119">2 </span><span class="sxs-lookup"><span data-stu-id="5c641-119">2</span></span>|<span data-ttu-id="5c641-120">任务已被接受，正在进行处理。</span><span class="sxs-lookup"><span data-stu-id="5c641-120">The task has been accepted and is being worked on.</span></span>|
|<span data-ttu-id="5c641-121">后</span><span class="sxs-lookup"><span data-stu-id="5c641-121">completed</span></span>|<span data-ttu-id="5c641-122">第三章</span><span class="sxs-lookup"><span data-stu-id="5c641-122">3</span></span>|<span data-ttu-id="5c641-123">工作已完成。</span><span class="sxs-lookup"><span data-stu-id="5c641-123">The work is complete.</span></span>|
|<span data-ttu-id="5c641-124">拒绝</span><span class="sxs-lookup"><span data-stu-id="5c641-124">rejected</span></span>|<span data-ttu-id="5c641-125">4 </span><span class="sxs-lookup"><span data-stu-id="5c641-125">4</span></span>|<span data-ttu-id="5c641-126">任务已被拒绝。</span><span class="sxs-lookup"><span data-stu-id="5c641-126">The task was rejected.</span></span>|






