---
title: complianceState 枚举类型
description: 合规性状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1c243145ee8511edb001ba2a55b3f72dde070297
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451284"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="d1405-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d1405-103">complianceState enum type</span></span>

<span data-ttu-id="d1405-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1405-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1405-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1405-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1405-106">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="d1405-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="d1405-107">成员</span><span class="sxs-lookup"><span data-stu-id="d1405-107">Members</span></span>
|<span data-ttu-id="d1405-108">成员</span><span class="sxs-lookup"><span data-stu-id="d1405-108">Member</span></span>|<span data-ttu-id="d1405-109">值</span><span class="sxs-lookup"><span data-stu-id="d1405-109">Value</span></span>|<span data-ttu-id="d1405-110">说明</span><span class="sxs-lookup"><span data-stu-id="d1405-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1405-111">unknown</span><span class="sxs-lookup"><span data-stu-id="d1405-111">unknown</span></span>|<span data-ttu-id="d1405-112">0</span><span class="sxs-lookup"><span data-stu-id="d1405-112">0</span></span>|<span data-ttu-id="d1405-113">陌生.</span><span class="sxs-lookup"><span data-stu-id="d1405-113">Unknown.</span></span>|
|<span data-ttu-id="d1405-114">合格</span><span class="sxs-lookup"><span data-stu-id="d1405-114">compliant</span></span>|<span data-ttu-id="d1405-115">1</span><span class="sxs-lookup"><span data-stu-id="d1405-115">1</span></span>|<span data-ttu-id="d1405-116">合格.</span><span class="sxs-lookup"><span data-stu-id="d1405-116">Compliant.</span></span>|
|<span data-ttu-id="d1405-117">合规</span><span class="sxs-lookup"><span data-stu-id="d1405-117">noncompliant</span></span>|<span data-ttu-id="d1405-118">双面</span><span class="sxs-lookup"><span data-stu-id="d1405-118">2</span></span>|<span data-ttu-id="d1405-119">设备不合规，并将从公司资源中阻止。</span><span class="sxs-lookup"><span data-stu-id="d1405-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="d1405-120">冲突</span><span class="sxs-lookup"><span data-stu-id="d1405-120">conflict</span></span>|<span data-ttu-id="d1405-121">第三章</span><span class="sxs-lookup"><span data-stu-id="d1405-121">3</span></span>|<span data-ttu-id="d1405-122">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="d1405-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="d1405-123">error</span><span class="sxs-lookup"><span data-stu-id="d1405-123">error</span></span>|<span data-ttu-id="d1405-124">4 </span><span class="sxs-lookup"><span data-stu-id="d1405-124">4</span></span>|<span data-ttu-id="d1405-125">错误。</span><span class="sxs-lookup"><span data-stu-id="d1405-125">Error.</span></span>|
|<span data-ttu-id="d1405-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="d1405-126">inGracePeriod</span></span>|<span data-ttu-id="d1405-127">254</span><span class="sxs-lookup"><span data-stu-id="d1405-127">254</span></span>|<span data-ttu-id="d1405-128">Device 不合规，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="d1405-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="d1405-129">configManager</span><span class="sxs-lookup"><span data-stu-id="d1405-129">configManager</span></span>|<span data-ttu-id="d1405-130">255</span><span class="sxs-lookup"><span data-stu-id="d1405-130">255</span></span>|<span data-ttu-id="d1405-131">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="d1405-131">Managed by Config Manager</span></span>|







