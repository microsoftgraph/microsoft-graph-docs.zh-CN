---
title: complianceState 枚举类型
description: 合规性状态。
author: tfitzmac
ms.openlocfilehash: 3fa0548c2a67aa5def5f859014f52e97bdda815b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321229"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="9d076-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9d076-103">complianceState enum type</span></span>

> <span data-ttu-id="9d076-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9d076-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d076-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9d076-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d076-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9d076-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d076-107">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="9d076-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="9d076-108">成员</span><span class="sxs-lookup"><span data-stu-id="9d076-108">Members</span></span>
|<span data-ttu-id="9d076-109">成员</span><span class="sxs-lookup"><span data-stu-id="9d076-109">Member</span></span>|<span data-ttu-id="9d076-110">值</span><span class="sxs-lookup"><span data-stu-id="9d076-110">Value</span></span>|<span data-ttu-id="9d076-111">说明</span><span class="sxs-lookup"><span data-stu-id="9d076-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d076-112">unknown</span><span class="sxs-lookup"><span data-stu-id="9d076-112">unknown</span></span>|<span data-ttu-id="9d076-113">0</span><span class="sxs-lookup"><span data-stu-id="9d076-113">0</span></span>|<span data-ttu-id="9d076-114">未知。</span><span class="sxs-lookup"><span data-stu-id="9d076-114">Unknown.</span></span>|
|<span data-ttu-id="9d076-115">符合标准</span><span class="sxs-lookup"><span data-stu-id="9d076-115">compliant</span></span>|<span data-ttu-id="9d076-116">1</span><span class="sxs-lookup"><span data-stu-id="9d076-116">1</span></span>|<span data-ttu-id="9d076-117">兼容。</span><span class="sxs-lookup"><span data-stu-id="9d076-117">Compliant.</span></span>|
|<span data-ttu-id="9d076-118">不符合标准</span><span class="sxs-lookup"><span data-stu-id="9d076-118">noncompliant</span></span>|<span data-ttu-id="9d076-119">2</span><span class="sxs-lookup"><span data-stu-id="9d076-119">2</span></span>|<span data-ttu-id="9d076-120">设备不兼容，并阻止从企业资源。</span><span class="sxs-lookup"><span data-stu-id="9d076-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="9d076-121">冲突</span><span class="sxs-lookup"><span data-stu-id="9d076-121">conflict</span></span>|<span data-ttu-id="9d076-122">3</span><span class="sxs-lookup"><span data-stu-id="9d076-122">3</span></span>|<span data-ttu-id="9d076-123">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="9d076-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="9d076-124">error</span><span class="sxs-lookup"><span data-stu-id="9d076-124">error</span></span>|<span data-ttu-id="9d076-125">4</span><span class="sxs-lookup"><span data-stu-id="9d076-125">4</span></span>|<span data-ttu-id="9d076-126">错误。</span><span class="sxs-lookup"><span data-stu-id="9d076-126">Error.</span></span>|
|<span data-ttu-id="9d076-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="9d076-127">inGracePeriod</span></span>|<span data-ttu-id="9d076-128">254</span><span class="sxs-lookup"><span data-stu-id="9d076-128">254</span></span>|<span data-ttu-id="9d076-129">设备不兼容，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="9d076-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="9d076-130">configManager</span><span class="sxs-lookup"><span data-stu-id="9d076-130">configManager</span></span>|<span data-ttu-id="9d076-131">255</span><span class="sxs-lookup"><span data-stu-id="9d076-131">255</span></span>|<span data-ttu-id="9d076-132">配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="9d076-132">Managed by Config Manager</span></span>|





