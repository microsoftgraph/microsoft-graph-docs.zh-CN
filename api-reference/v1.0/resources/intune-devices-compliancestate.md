---
title: complianceState 枚举类型
description: 合规性状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d578417c616fc2dbf30b8fe95d2f58ede5fd3df2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253356"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="63c1b-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="63c1b-103">complianceState enum type</span></span>

> <span data-ttu-id="63c1b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63c1b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63c1b-105">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="63c1b-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="63c1b-106">成员</span><span class="sxs-lookup"><span data-stu-id="63c1b-106">Members</span></span>
|<span data-ttu-id="63c1b-107">成员</span><span class="sxs-lookup"><span data-stu-id="63c1b-107">Member</span></span>|<span data-ttu-id="63c1b-108">值</span><span class="sxs-lookup"><span data-stu-id="63c1b-108">Value</span></span>|<span data-ttu-id="63c1b-109">说明</span><span class="sxs-lookup"><span data-stu-id="63c1b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63c1b-110">unknown</span><span class="sxs-lookup"><span data-stu-id="63c1b-110">unknown</span></span>|<span data-ttu-id="63c1b-111">0</span><span class="sxs-lookup"><span data-stu-id="63c1b-111">0</span></span>|<span data-ttu-id="63c1b-112">陌生.</span><span class="sxs-lookup"><span data-stu-id="63c1b-112">Unknown.</span></span>|
|<span data-ttu-id="63c1b-113">合格</span><span class="sxs-lookup"><span data-stu-id="63c1b-113">compliant</span></span>|<span data-ttu-id="63c1b-114">1</span><span class="sxs-lookup"><span data-stu-id="63c1b-114">1</span></span>|<span data-ttu-id="63c1b-115">合格.</span><span class="sxs-lookup"><span data-stu-id="63c1b-115">Compliant.</span></span>|
|<span data-ttu-id="63c1b-116">合规</span><span class="sxs-lookup"><span data-stu-id="63c1b-116">noncompliant</span></span>|<span data-ttu-id="63c1b-117">双面</span><span class="sxs-lookup"><span data-stu-id="63c1b-117">2</span></span>|<span data-ttu-id="63c1b-118">设备不合规, 并将从公司资源中阻止。</span><span class="sxs-lookup"><span data-stu-id="63c1b-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="63c1b-119">冲突</span><span class="sxs-lookup"><span data-stu-id="63c1b-119">conflict</span></span>|<span data-ttu-id="63c1b-120">第三章</span><span class="sxs-lookup"><span data-stu-id="63c1b-120">3</span></span>|<span data-ttu-id="63c1b-121">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="63c1b-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="63c1b-122">error</span><span class="sxs-lookup"><span data-stu-id="63c1b-122">error</span></span>|<span data-ttu-id="63c1b-123">4</span><span class="sxs-lookup"><span data-stu-id="63c1b-123">4</span></span>|<span data-ttu-id="63c1b-124">错误。</span><span class="sxs-lookup"><span data-stu-id="63c1b-124">Error.</span></span>|
|<span data-ttu-id="63c1b-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="63c1b-125">inGracePeriod</span></span>|<span data-ttu-id="63c1b-126">254</span><span class="sxs-lookup"><span data-stu-id="63c1b-126">254</span></span>|<span data-ttu-id="63c1b-127">Device 不合规, 但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="63c1b-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="63c1b-128">configManager</span><span class="sxs-lookup"><span data-stu-id="63c1b-128">configManager</span></span>|<span data-ttu-id="63c1b-129">255</span><span class="sxs-lookup"><span data-stu-id="63c1b-129">255</span></span>|<span data-ttu-id="63c1b-130">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="63c1b-130">Managed by Config Manager</span></span>|



