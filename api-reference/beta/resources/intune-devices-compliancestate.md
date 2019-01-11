---
title: complianceState 枚举类型
description: 合规性状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b3d496d6890d0da4d817ad9ba1f03e4b0825204d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861675"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="f981f-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f981f-103">complianceState enum type</span></span>

> <span data-ttu-id="f981f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f981f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f981f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f981f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f981f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f981f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f981f-107">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="f981f-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="f981f-108">成员</span><span class="sxs-lookup"><span data-stu-id="f981f-108">Members</span></span>
|<span data-ttu-id="f981f-109">成员</span><span class="sxs-lookup"><span data-stu-id="f981f-109">Member</span></span>|<span data-ttu-id="f981f-110">值</span><span class="sxs-lookup"><span data-stu-id="f981f-110">Value</span></span>|<span data-ttu-id="f981f-111">Description</span><span class="sxs-lookup"><span data-stu-id="f981f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f981f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="f981f-112">unknown</span></span>|<span data-ttu-id="f981f-113">0</span><span class="sxs-lookup"><span data-stu-id="f981f-113">0</span></span>|<span data-ttu-id="f981f-114">未知。</span><span class="sxs-lookup"><span data-stu-id="f981f-114">Unknown.</span></span>|
|<span data-ttu-id="f981f-115">符合标准</span><span class="sxs-lookup"><span data-stu-id="f981f-115">compliant</span></span>|<span data-ttu-id="f981f-116">1</span><span class="sxs-lookup"><span data-stu-id="f981f-116">1</span></span>|<span data-ttu-id="f981f-117">兼容。</span><span class="sxs-lookup"><span data-stu-id="f981f-117">Compliant.</span></span>|
|<span data-ttu-id="f981f-118">不符合标准</span><span class="sxs-lookup"><span data-stu-id="f981f-118">noncompliant</span></span>|<span data-ttu-id="f981f-119">2</span><span class="sxs-lookup"><span data-stu-id="f981f-119">2</span></span>|<span data-ttu-id="f981f-120">设备不兼容，并阻止从企业资源。</span><span class="sxs-lookup"><span data-stu-id="f981f-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="f981f-121">冲突</span><span class="sxs-lookup"><span data-stu-id="f981f-121">conflict</span></span>|<span data-ttu-id="f981f-122">3</span><span class="sxs-lookup"><span data-stu-id="f981f-122">3</span></span>|<span data-ttu-id="f981f-123">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="f981f-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="f981f-124">error</span><span class="sxs-lookup"><span data-stu-id="f981f-124">error</span></span>|<span data-ttu-id="f981f-125">4</span><span class="sxs-lookup"><span data-stu-id="f981f-125">4</span></span>|<span data-ttu-id="f981f-126">错误。</span><span class="sxs-lookup"><span data-stu-id="f981f-126">Error.</span></span>|
|<span data-ttu-id="f981f-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="f981f-127">inGracePeriod</span></span>|<span data-ttu-id="f981f-128">254</span><span class="sxs-lookup"><span data-stu-id="f981f-128">254</span></span>|<span data-ttu-id="f981f-129">设备不兼容，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="f981f-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="f981f-130">configManager</span><span class="sxs-lookup"><span data-stu-id="f981f-130">configManager</span></span>|<span data-ttu-id="f981f-131">255</span><span class="sxs-lookup"><span data-stu-id="f981f-131">255</span></span>|<span data-ttu-id="f981f-132">配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="f981f-132">Managed by Config Manager</span></span>|





