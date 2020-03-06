---
title: complianceState 枚举类型
description: 合规性状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b0b20615dfdda489649182d0c0687e9a735b5f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532225"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="2801a-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2801a-103">complianceState enum type</span></span>

<span data-ttu-id="2801a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2801a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2801a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2801a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2801a-106">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="2801a-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="2801a-107">成员</span><span class="sxs-lookup"><span data-stu-id="2801a-107">Members</span></span>
|<span data-ttu-id="2801a-108">成员</span><span class="sxs-lookup"><span data-stu-id="2801a-108">Member</span></span>|<span data-ttu-id="2801a-109">值</span><span class="sxs-lookup"><span data-stu-id="2801a-109">Value</span></span>|<span data-ttu-id="2801a-110">说明</span><span class="sxs-lookup"><span data-stu-id="2801a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2801a-111">unknown</span><span class="sxs-lookup"><span data-stu-id="2801a-111">unknown</span></span>|<span data-ttu-id="2801a-112">0</span><span class="sxs-lookup"><span data-stu-id="2801a-112">0</span></span>|<span data-ttu-id="2801a-113">陌生.</span><span class="sxs-lookup"><span data-stu-id="2801a-113">Unknown.</span></span>|
|<span data-ttu-id="2801a-114">合格</span><span class="sxs-lookup"><span data-stu-id="2801a-114">compliant</span></span>|<span data-ttu-id="2801a-115">1 </span><span class="sxs-lookup"><span data-stu-id="2801a-115">1</span></span>|<span data-ttu-id="2801a-116">合格.</span><span class="sxs-lookup"><span data-stu-id="2801a-116">Compliant.</span></span>|
|<span data-ttu-id="2801a-117">合规</span><span class="sxs-lookup"><span data-stu-id="2801a-117">noncompliant</span></span>|<span data-ttu-id="2801a-118">2 </span><span class="sxs-lookup"><span data-stu-id="2801a-118">2</span></span>|<span data-ttu-id="2801a-119">设备不合规，并将从公司资源中阻止。</span><span class="sxs-lookup"><span data-stu-id="2801a-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="2801a-120">冲突</span><span class="sxs-lookup"><span data-stu-id="2801a-120">conflict</span></span>|<span data-ttu-id="2801a-121">3 </span><span class="sxs-lookup"><span data-stu-id="2801a-121">3</span></span>|<span data-ttu-id="2801a-122">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="2801a-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="2801a-123">error</span><span class="sxs-lookup"><span data-stu-id="2801a-123">error</span></span>|<span data-ttu-id="2801a-124">4 </span><span class="sxs-lookup"><span data-stu-id="2801a-124">4</span></span>|<span data-ttu-id="2801a-125">错误。</span><span class="sxs-lookup"><span data-stu-id="2801a-125">Error.</span></span>|
|<span data-ttu-id="2801a-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="2801a-126">inGracePeriod</span></span>|<span data-ttu-id="2801a-127">254</span><span class="sxs-lookup"><span data-stu-id="2801a-127">254</span></span>|<span data-ttu-id="2801a-128">Device 不合规，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="2801a-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="2801a-129">configManager</span><span class="sxs-lookup"><span data-stu-id="2801a-129">configManager</span></span>|<span data-ttu-id="2801a-130">255</span><span class="sxs-lookup"><span data-stu-id="2801a-130">255</span></span>|<span data-ttu-id="2801a-131">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="2801a-131">Managed by Config Manager</span></span>|




