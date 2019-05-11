---
title: complianceState 枚举类型
description: 合规性状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6dc39839754f24ae25044b0aa249d61fe2655d68
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943031"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="910ed-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="910ed-103">complianceState enum type</span></span>

> <span data-ttu-id="910ed-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="910ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="910ed-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="910ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="910ed-106">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="910ed-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="910ed-107">成员</span><span class="sxs-lookup"><span data-stu-id="910ed-107">Members</span></span>
|<span data-ttu-id="910ed-108">成员</span><span class="sxs-lookup"><span data-stu-id="910ed-108">Member</span></span>|<span data-ttu-id="910ed-109">值</span><span class="sxs-lookup"><span data-stu-id="910ed-109">Value</span></span>|<span data-ttu-id="910ed-110">说明</span><span class="sxs-lookup"><span data-stu-id="910ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="910ed-111">unknown</span><span class="sxs-lookup"><span data-stu-id="910ed-111">unknown</span></span>|<span data-ttu-id="910ed-112">0</span><span class="sxs-lookup"><span data-stu-id="910ed-112">0</span></span>|<span data-ttu-id="910ed-113">陌生.</span><span class="sxs-lookup"><span data-stu-id="910ed-113">Unknown.</span></span>|
|<span data-ttu-id="910ed-114">合格</span><span class="sxs-lookup"><span data-stu-id="910ed-114">compliant</span></span>|<span data-ttu-id="910ed-115">1</span><span class="sxs-lookup"><span data-stu-id="910ed-115">1</span></span>|<span data-ttu-id="910ed-116">合格.</span><span class="sxs-lookup"><span data-stu-id="910ed-116">Compliant.</span></span>|
|<span data-ttu-id="910ed-117">合规</span><span class="sxs-lookup"><span data-stu-id="910ed-117">noncompliant</span></span>|<span data-ttu-id="910ed-118">双面</span><span class="sxs-lookup"><span data-stu-id="910ed-118">2</span></span>|<span data-ttu-id="910ed-119">设备不合规, 并将从公司资源中阻止。</span><span class="sxs-lookup"><span data-stu-id="910ed-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="910ed-120">冲突</span><span class="sxs-lookup"><span data-stu-id="910ed-120">conflict</span></span>|<span data-ttu-id="910ed-121">第三章</span><span class="sxs-lookup"><span data-stu-id="910ed-121">3</span></span>|<span data-ttu-id="910ed-122">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="910ed-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="910ed-123">error</span><span class="sxs-lookup"><span data-stu-id="910ed-123">error</span></span>|<span data-ttu-id="910ed-124">4</span><span class="sxs-lookup"><span data-stu-id="910ed-124">4</span></span>|<span data-ttu-id="910ed-125">错误。</span><span class="sxs-lookup"><span data-stu-id="910ed-125">Error.</span></span>|
|<span data-ttu-id="910ed-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="910ed-126">inGracePeriod</span></span>|<span data-ttu-id="910ed-127">254</span><span class="sxs-lookup"><span data-stu-id="910ed-127">254</span></span>|<span data-ttu-id="910ed-128">Device 不合规, 但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="910ed-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="910ed-129">configManager</span><span class="sxs-lookup"><span data-stu-id="910ed-129">configManager</span></span>|<span data-ttu-id="910ed-130">255</span><span class="sxs-lookup"><span data-stu-id="910ed-130">255</span></span>|<span data-ttu-id="910ed-131">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="910ed-131">Managed by Config Manager</span></span>|




