---
title: deviceAppManagementTaskStatus 枚举类型
description: 设备应用程序管理任务状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3bcd6dcf957748a0e57776bd318cdb1ee734172
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002586"
---
# <a name="deviceappmanagementtaskstatus-enum-type"></a><span data-ttu-id="df218-103">deviceAppManagementTaskStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="df218-103">deviceAppManagementTaskStatus enum type</span></span>

> <span data-ttu-id="df218-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df218-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df218-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df218-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df218-106">设备应用程序管理任务状态。</span><span class="sxs-lookup"><span data-stu-id="df218-106">Device app management task status.</span></span>

## <a name="members"></a><span data-ttu-id="df218-107">成员</span><span class="sxs-lookup"><span data-stu-id="df218-107">Members</span></span>
|<span data-ttu-id="df218-108">成员</span><span class="sxs-lookup"><span data-stu-id="df218-108">Member</span></span>|<span data-ttu-id="df218-109">值</span><span class="sxs-lookup"><span data-stu-id="df218-109">Value</span></span>|<span data-ttu-id="df218-110">说明</span><span class="sxs-lookup"><span data-stu-id="df218-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df218-111">unknown</span><span class="sxs-lookup"><span data-stu-id="df218-111">unknown</span></span>|<span data-ttu-id="df218-112">0</span><span class="sxs-lookup"><span data-stu-id="df218-112">0</span></span>|<span data-ttu-id="df218-113">状态未定义。</span><span class="sxs-lookup"><span data-stu-id="df218-113">State is undefined.</span></span>|
|<span data-ttu-id="df218-114">决</span><span class="sxs-lookup"><span data-stu-id="df218-114">pending</span></span>|<span data-ttu-id="df218-115">1</span><span class="sxs-lookup"><span data-stu-id="df218-115">1</span></span>|<span data-ttu-id="df218-116">任务已准备好进行审阅。</span><span class="sxs-lookup"><span data-stu-id="df218-116">The task is ready for review.</span></span>|
|<span data-ttu-id="df218-117">工作</span><span class="sxs-lookup"><span data-stu-id="df218-117">active</span></span>|<span data-ttu-id="df218-118">双面</span><span class="sxs-lookup"><span data-stu-id="df218-118">2</span></span>|<span data-ttu-id="df218-119">任务已被接受, 正在进行处理。</span><span class="sxs-lookup"><span data-stu-id="df218-119">The task has been accepted and is being worked on.</span></span>|
|<span data-ttu-id="df218-120">后</span><span class="sxs-lookup"><span data-stu-id="df218-120">completed</span></span>|<span data-ttu-id="df218-121">第三章</span><span class="sxs-lookup"><span data-stu-id="df218-121">3</span></span>|<span data-ttu-id="df218-122">工作已完成。</span><span class="sxs-lookup"><span data-stu-id="df218-122">The work is complete.</span></span>|
|<span data-ttu-id="df218-123">拒绝</span><span class="sxs-lookup"><span data-stu-id="df218-123">rejected</span></span>|<span data-ttu-id="df218-124">4</span><span class="sxs-lookup"><span data-stu-id="df218-124">4</span></span>|<span data-ttu-id="df218-125">任务已被拒绝。</span><span class="sxs-lookup"><span data-stu-id="df218-125">The task was rejected.</span></span>|





