---
title: complianceState 枚举类型
description: 合规性状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 01c0a3443eae87fb69b4b6482a2da2c2e067c5d1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357057"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="5e0a1-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5e0a1-103">complianceState enum type</span></span>

> <span data-ttu-id="5e0a1-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e0a1-105">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="5e0a1-106">成员</span><span class="sxs-lookup"><span data-stu-id="5e0a1-106">Members</span></span>
|<span data-ttu-id="5e0a1-107">成员</span><span class="sxs-lookup"><span data-stu-id="5e0a1-107">Member</span></span>|<span data-ttu-id="5e0a1-108">值</span><span class="sxs-lookup"><span data-stu-id="5e0a1-108">Value</span></span>|<span data-ttu-id="5e0a1-109">说明</span><span class="sxs-lookup"><span data-stu-id="5e0a1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e0a1-110">unknown</span><span class="sxs-lookup"><span data-stu-id="5e0a1-110">unknown</span></span>|<span data-ttu-id="5e0a1-111">0</span><span class="sxs-lookup"><span data-stu-id="5e0a1-111">0</span></span>|<span data-ttu-id="5e0a1-112">陌生.</span><span class="sxs-lookup"><span data-stu-id="5e0a1-112">Unknown.</span></span>|
|<span data-ttu-id="5e0a1-113">合格</span><span class="sxs-lookup"><span data-stu-id="5e0a1-113">compliant</span></span>|<span data-ttu-id="5e0a1-114">1</span><span class="sxs-lookup"><span data-stu-id="5e0a1-114">1</span></span>|<span data-ttu-id="5e0a1-115">合格.</span><span class="sxs-lookup"><span data-stu-id="5e0a1-115">Compliant.</span></span>|
|<span data-ttu-id="5e0a1-116">合规</span><span class="sxs-lookup"><span data-stu-id="5e0a1-116">noncompliant</span></span>|<span data-ttu-id="5e0a1-117">双面</span><span class="sxs-lookup"><span data-stu-id="5e0a1-117">2</span></span>|<span data-ttu-id="5e0a1-118">设备不合规，并将从公司资源中阻止。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="5e0a1-119">冲突</span><span class="sxs-lookup"><span data-stu-id="5e0a1-119">conflict</span></span>|<span data-ttu-id="5e0a1-120">第三章</span><span class="sxs-lookup"><span data-stu-id="5e0a1-120">3</span></span>|<span data-ttu-id="5e0a1-121">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="5e0a1-122">error</span><span class="sxs-lookup"><span data-stu-id="5e0a1-122">error</span></span>|<span data-ttu-id="5e0a1-123">4</span><span class="sxs-lookup"><span data-stu-id="5e0a1-123">4</span></span>|<span data-ttu-id="5e0a1-124">错误。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-124">Error.</span></span>|
|<span data-ttu-id="5e0a1-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="5e0a1-125">inGracePeriod</span></span>|<span data-ttu-id="5e0a1-126">254</span><span class="sxs-lookup"><span data-stu-id="5e0a1-126">254</span></span>|<span data-ttu-id="5e0a1-127">Device 不合规，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="5e0a1-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="5e0a1-128">configManager</span><span class="sxs-lookup"><span data-stu-id="5e0a1-128">configManager</span></span>|<span data-ttu-id="5e0a1-129">255</span><span class="sxs-lookup"><span data-stu-id="5e0a1-129">255</span></span>|<span data-ttu-id="5e0a1-130">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="5e0a1-130">Managed by Config Manager</span></span>|




