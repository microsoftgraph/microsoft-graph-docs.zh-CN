---
title: deviceAppManagementTaskStatus 枚举类型
description: 设备应用程序管理任务状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1302bec464f92a19d96746c11e3c858a00332e8d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730407"
---
# <a name="deviceappmanagementtaskstatus-enum-type"></a><span data-ttu-id="d53bf-103">deviceAppManagementTaskStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d53bf-103">deviceAppManagementTaskStatus enum type</span></span>

<span data-ttu-id="d53bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d53bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d53bf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d53bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d53bf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d53bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d53bf-107">设备应用程序管理任务状态。</span><span class="sxs-lookup"><span data-stu-id="d53bf-107">Device app management task status.</span></span>

## <a name="members"></a><span data-ttu-id="d53bf-108">成员</span><span class="sxs-lookup"><span data-stu-id="d53bf-108">Members</span></span>
|<span data-ttu-id="d53bf-109">成员</span><span class="sxs-lookup"><span data-stu-id="d53bf-109">Member</span></span>|<span data-ttu-id="d53bf-110">值</span><span class="sxs-lookup"><span data-stu-id="d53bf-110">Value</span></span>|<span data-ttu-id="d53bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="d53bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d53bf-112">unknown</span><span class="sxs-lookup"><span data-stu-id="d53bf-112">unknown</span></span>|<span data-ttu-id="d53bf-113">0</span><span class="sxs-lookup"><span data-stu-id="d53bf-113">0</span></span>|<span data-ttu-id="d53bf-114">状态未定义。</span><span class="sxs-lookup"><span data-stu-id="d53bf-114">State is undefined.</span></span>|
|<span data-ttu-id="d53bf-115">决</span><span class="sxs-lookup"><span data-stu-id="d53bf-115">pending</span></span>|<span data-ttu-id="d53bf-116">1</span><span class="sxs-lookup"><span data-stu-id="d53bf-116">1</span></span>|<span data-ttu-id="d53bf-117">任务已准备好进行审阅。</span><span class="sxs-lookup"><span data-stu-id="d53bf-117">The task is ready for review.</span></span>|
|<span data-ttu-id="d53bf-118">工作</span><span class="sxs-lookup"><span data-stu-id="d53bf-118">active</span></span>|<span data-ttu-id="d53bf-119">双面</span><span class="sxs-lookup"><span data-stu-id="d53bf-119">2</span></span>|<span data-ttu-id="d53bf-120">任务已被接受，正在进行处理。</span><span class="sxs-lookup"><span data-stu-id="d53bf-120">The task has been accepted and is being worked on.</span></span>|
|<span data-ttu-id="d53bf-121">后</span><span class="sxs-lookup"><span data-stu-id="d53bf-121">completed</span></span>|<span data-ttu-id="d53bf-122">第三章</span><span class="sxs-lookup"><span data-stu-id="d53bf-122">3</span></span>|<span data-ttu-id="d53bf-123">工作已完成。</span><span class="sxs-lookup"><span data-stu-id="d53bf-123">The work is complete.</span></span>|
|<span data-ttu-id="d53bf-124">拒绝</span><span class="sxs-lookup"><span data-stu-id="d53bf-124">rejected</span></span>|<span data-ttu-id="d53bf-125">4 </span><span class="sxs-lookup"><span data-stu-id="d53bf-125">4</span></span>|<span data-ttu-id="d53bf-126">任务已被拒绝。</span><span class="sxs-lookup"><span data-stu-id="d53bf-126">The task was rejected.</span></span>|





