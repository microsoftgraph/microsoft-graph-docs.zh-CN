---
title: deviceAppManagementTaskStatus 枚举类型
description: 设备应用程序管理任务状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7e16d4904e8c81209190cca4ccd3d8304fcdfff2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308167"
---
# <a name="deviceappmanagementtaskstatus-enum-type"></a><span data-ttu-id="455df-103">deviceAppManagementTaskStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="455df-103">deviceAppManagementTaskStatus enum type</span></span>

> <span data-ttu-id="455df-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="455df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="455df-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="455df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="455df-106">设备应用程序管理任务状态。</span><span class="sxs-lookup"><span data-stu-id="455df-106">Device app management task status.</span></span>

## <a name="members"></a><span data-ttu-id="455df-107">成员</span><span class="sxs-lookup"><span data-stu-id="455df-107">Members</span></span>
|<span data-ttu-id="455df-108">成员</span><span class="sxs-lookup"><span data-stu-id="455df-108">Member</span></span>|<span data-ttu-id="455df-109">值</span><span class="sxs-lookup"><span data-stu-id="455df-109">Value</span></span>|<span data-ttu-id="455df-110">说明</span><span class="sxs-lookup"><span data-stu-id="455df-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="455df-111">unknown</span><span class="sxs-lookup"><span data-stu-id="455df-111">unknown</span></span>|<span data-ttu-id="455df-112">0</span><span class="sxs-lookup"><span data-stu-id="455df-112">0</span></span>|<span data-ttu-id="455df-113">状态未定义。</span><span class="sxs-lookup"><span data-stu-id="455df-113">State is undefined.</span></span>|
|<span data-ttu-id="455df-114">决</span><span class="sxs-lookup"><span data-stu-id="455df-114">pending</span></span>|<span data-ttu-id="455df-115">1</span><span class="sxs-lookup"><span data-stu-id="455df-115">1</span></span>|<span data-ttu-id="455df-116">任务已准备好进行审阅。</span><span class="sxs-lookup"><span data-stu-id="455df-116">The task is ready for review.</span></span>|
|<span data-ttu-id="455df-117">工作</span><span class="sxs-lookup"><span data-stu-id="455df-117">active</span></span>|<span data-ttu-id="455df-118">双面</span><span class="sxs-lookup"><span data-stu-id="455df-118">2</span></span>|<span data-ttu-id="455df-119">任务已被接受, 正在进行处理。</span><span class="sxs-lookup"><span data-stu-id="455df-119">The task has been accepted and is being worked on.</span></span>|
|<span data-ttu-id="455df-120">后</span><span class="sxs-lookup"><span data-stu-id="455df-120">completed</span></span>|<span data-ttu-id="455df-121">第三章</span><span class="sxs-lookup"><span data-stu-id="455df-121">3</span></span>|<span data-ttu-id="455df-122">工作已完成。</span><span class="sxs-lookup"><span data-stu-id="455df-122">The work is complete.</span></span>|
|<span data-ttu-id="455df-123">拒绝</span><span class="sxs-lookup"><span data-stu-id="455df-123">rejected</span></span>|<span data-ttu-id="455df-124">4</span><span class="sxs-lookup"><span data-stu-id="455df-124">4</span></span>|<span data-ttu-id="455df-125">任务已被拒绝。</span><span class="sxs-lookup"><span data-stu-id="455df-125">The task was rejected.</span></span>|



