---
title: complianceState 枚举类型
description: 合规性状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53b17f258f577e0842dbfc81c6341303f6b43799
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820340"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="09e53-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="09e53-103">complianceState enum type</span></span>

> <span data-ttu-id="09e53-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="09e53-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09e53-105">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="09e53-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="09e53-106">成员</span><span class="sxs-lookup"><span data-stu-id="09e53-106">Members</span></span>
|<span data-ttu-id="09e53-107">成员</span><span class="sxs-lookup"><span data-stu-id="09e53-107">Member</span></span>|<span data-ttu-id="09e53-108">值</span><span class="sxs-lookup"><span data-stu-id="09e53-108">Value</span></span>|<span data-ttu-id="09e53-109">Description</span><span class="sxs-lookup"><span data-stu-id="09e53-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09e53-110">unknown</span><span class="sxs-lookup"><span data-stu-id="09e53-110">unknown</span></span>|<span data-ttu-id="09e53-111">0</span><span class="sxs-lookup"><span data-stu-id="09e53-111">0</span></span>|<span data-ttu-id="09e53-112">未知。</span><span class="sxs-lookup"><span data-stu-id="09e53-112">Unknown.</span></span>|
|<span data-ttu-id="09e53-113">符合标准</span><span class="sxs-lookup"><span data-stu-id="09e53-113">compliant</span></span>|<span data-ttu-id="09e53-114">1</span><span class="sxs-lookup"><span data-stu-id="09e53-114">1</span></span>|<span data-ttu-id="09e53-115">兼容。</span><span class="sxs-lookup"><span data-stu-id="09e53-115">Compliant.</span></span>|
|<span data-ttu-id="09e53-116">不符合标准</span><span class="sxs-lookup"><span data-stu-id="09e53-116">noncompliant</span></span>|<span data-ttu-id="09e53-117">2</span><span class="sxs-lookup"><span data-stu-id="09e53-117">2</span></span>|<span data-ttu-id="09e53-118">设备不兼容，并阻止从企业资源。</span><span class="sxs-lookup"><span data-stu-id="09e53-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="09e53-119">冲突</span><span class="sxs-lookup"><span data-stu-id="09e53-119">conflict</span></span>|<span data-ttu-id="09e53-120">3</span><span class="sxs-lookup"><span data-stu-id="09e53-120">3</span></span>|<span data-ttu-id="09e53-121">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="09e53-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="09e53-122">error</span><span class="sxs-lookup"><span data-stu-id="09e53-122">error</span></span>|<span data-ttu-id="09e53-123">4</span><span class="sxs-lookup"><span data-stu-id="09e53-123">4</span></span>|<span data-ttu-id="09e53-124">错误。</span><span class="sxs-lookup"><span data-stu-id="09e53-124">Error.</span></span>|
|<span data-ttu-id="09e53-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="09e53-125">inGracePeriod</span></span>|<span data-ttu-id="09e53-126">254</span><span class="sxs-lookup"><span data-stu-id="09e53-126">254</span></span>|<span data-ttu-id="09e53-127">设备不兼容，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="09e53-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="09e53-128">configManager</span><span class="sxs-lookup"><span data-stu-id="09e53-128">configManager</span></span>|<span data-ttu-id="09e53-129">255</span><span class="sxs-lookup"><span data-stu-id="09e53-129">255</span></span>|<span data-ttu-id="09e53-130">配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="09e53-130">Managed by Config Manager</span></span>|



