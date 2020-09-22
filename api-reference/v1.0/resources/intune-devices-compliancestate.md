---
title: complianceState 枚举类型
description: 合规性状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 24f7a2a62ae45504c03d2fcff49ca8f17bfab28b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091304"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="f8326-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f8326-103">complianceState enum type</span></span>

<span data-ttu-id="f8326-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8326-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8326-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8326-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8326-106">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="f8326-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="f8326-107">成员</span><span class="sxs-lookup"><span data-stu-id="f8326-107">Members</span></span>
|<span data-ttu-id="f8326-108">成员</span><span class="sxs-lookup"><span data-stu-id="f8326-108">Member</span></span>|<span data-ttu-id="f8326-109">值</span><span class="sxs-lookup"><span data-stu-id="f8326-109">Value</span></span>|<span data-ttu-id="f8326-110">说明</span><span class="sxs-lookup"><span data-stu-id="f8326-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8326-111">unknown</span><span class="sxs-lookup"><span data-stu-id="f8326-111">unknown</span></span>|<span data-ttu-id="f8326-112">0</span><span class="sxs-lookup"><span data-stu-id="f8326-112">0</span></span>|<span data-ttu-id="f8326-113">陌生.</span><span class="sxs-lookup"><span data-stu-id="f8326-113">Unknown.</span></span>|
|<span data-ttu-id="f8326-114">合格</span><span class="sxs-lookup"><span data-stu-id="f8326-114">compliant</span></span>|<span data-ttu-id="f8326-115">1 </span><span class="sxs-lookup"><span data-stu-id="f8326-115">1</span></span>|<span data-ttu-id="f8326-116">合格.</span><span class="sxs-lookup"><span data-stu-id="f8326-116">Compliant.</span></span>|
|<span data-ttu-id="f8326-117">合规</span><span class="sxs-lookup"><span data-stu-id="f8326-117">noncompliant</span></span>|<span data-ttu-id="f8326-118">2 </span><span class="sxs-lookup"><span data-stu-id="f8326-118">2</span></span>|<span data-ttu-id="f8326-119">设备不合规，并将从公司资源中阻止。</span><span class="sxs-lookup"><span data-stu-id="f8326-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="f8326-120">冲突</span><span class="sxs-lookup"><span data-stu-id="f8326-120">conflict</span></span>|<span data-ttu-id="f8326-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f8326-121">3</span></span>|<span data-ttu-id="f8326-122">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="f8326-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="f8326-123">error</span><span class="sxs-lookup"><span data-stu-id="f8326-123">error</span></span>|<span data-ttu-id="f8326-124">4 </span><span class="sxs-lookup"><span data-stu-id="f8326-124">4</span></span>|<span data-ttu-id="f8326-125">错误。</span><span class="sxs-lookup"><span data-stu-id="f8326-125">Error.</span></span>|
|<span data-ttu-id="f8326-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="f8326-126">inGracePeriod</span></span>|<span data-ttu-id="f8326-127">254</span><span class="sxs-lookup"><span data-stu-id="f8326-127">254</span></span>|<span data-ttu-id="f8326-128">Device 不合规，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="f8326-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="f8326-129">configManager</span><span class="sxs-lookup"><span data-stu-id="f8326-129">configManager</span></span>|<span data-ttu-id="f8326-130">255</span><span class="sxs-lookup"><span data-stu-id="f8326-130">255</span></span>|<span data-ttu-id="f8326-131">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="f8326-131">Managed by Config Manager</span></span>|









