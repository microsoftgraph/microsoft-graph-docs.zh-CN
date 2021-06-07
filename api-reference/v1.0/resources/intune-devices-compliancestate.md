---
title: complianceState 枚举类型
description: 合规性状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4bae464724712333c81b73bdcd23e57148655624
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757736"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="b48bd-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b48bd-103">complianceState enum type</span></span>

<span data-ttu-id="b48bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b48bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b48bd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b48bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b48bd-106">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="b48bd-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="b48bd-107">成员</span><span class="sxs-lookup"><span data-stu-id="b48bd-107">Members</span></span>
|<span data-ttu-id="b48bd-108">成员</span><span class="sxs-lookup"><span data-stu-id="b48bd-108">Member</span></span>|<span data-ttu-id="b48bd-109">值</span><span class="sxs-lookup"><span data-stu-id="b48bd-109">Value</span></span>|<span data-ttu-id="b48bd-110">Description</span><span class="sxs-lookup"><span data-stu-id="b48bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b48bd-111">unknown</span><span class="sxs-lookup"><span data-stu-id="b48bd-111">unknown</span></span>|<span data-ttu-id="b48bd-112">0</span><span class="sxs-lookup"><span data-stu-id="b48bd-112">0</span></span>|<span data-ttu-id="b48bd-113">未知。</span><span class="sxs-lookup"><span data-stu-id="b48bd-113">Unknown.</span></span>|
|<span data-ttu-id="b48bd-114">compliant</span><span class="sxs-lookup"><span data-stu-id="b48bd-114">compliant</span></span>|<span data-ttu-id="b48bd-115">1</span><span class="sxs-lookup"><span data-stu-id="b48bd-115">1</span></span>|<span data-ttu-id="b48bd-116">兼容。</span><span class="sxs-lookup"><span data-stu-id="b48bd-116">Compliant.</span></span>|
|<span data-ttu-id="b48bd-117">不符合</span><span class="sxs-lookup"><span data-stu-id="b48bd-117">noncompliant</span></span>|<span data-ttu-id="b48bd-118">2</span><span class="sxs-lookup"><span data-stu-id="b48bd-118">2</span></span>|<span data-ttu-id="b48bd-119">设备不兼容，并且被阻止访问公司资源。</span><span class="sxs-lookup"><span data-stu-id="b48bd-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="b48bd-120">conflict</span><span class="sxs-lookup"><span data-stu-id="b48bd-120">conflict</span></span>|<span data-ttu-id="b48bd-121">3</span><span class="sxs-lookup"><span data-stu-id="b48bd-121">3</span></span>|<span data-ttu-id="b48bd-122">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="b48bd-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="b48bd-123">error</span><span class="sxs-lookup"><span data-stu-id="b48bd-123">error</span></span>|<span data-ttu-id="b48bd-124">4 </span><span class="sxs-lookup"><span data-stu-id="b48bd-124">4</span></span>|<span data-ttu-id="b48bd-125">错误。</span><span class="sxs-lookup"><span data-stu-id="b48bd-125">Error.</span></span>|
|<span data-ttu-id="b48bd-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="b48bd-126">inGracePeriod</span></span>|<span data-ttu-id="b48bd-127">254</span><span class="sxs-lookup"><span data-stu-id="b48bd-127">254</span></span>|<span data-ttu-id="b48bd-128">设备不合规，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="b48bd-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="b48bd-129">configManager</span><span class="sxs-lookup"><span data-stu-id="b48bd-129">configManager</span></span>|<span data-ttu-id="b48bd-130">255</span><span class="sxs-lookup"><span data-stu-id="b48bd-130">255</span></span>|<span data-ttu-id="b48bd-131">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="b48bd-131">Managed by Config Manager</span></span>|




