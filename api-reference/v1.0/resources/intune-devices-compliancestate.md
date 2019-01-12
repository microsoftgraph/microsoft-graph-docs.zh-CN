---
title: complianceState 枚举类型
description: 合规性状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a4f4c359665eb1a0087f64802b5e7c829002fd6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940195"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="a49df-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a49df-103">complianceState enum type</span></span>

> <span data-ttu-id="a49df-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a49df-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a49df-105">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="a49df-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="a49df-106">成员</span><span class="sxs-lookup"><span data-stu-id="a49df-106">Members</span></span>
|<span data-ttu-id="a49df-107">成员</span><span class="sxs-lookup"><span data-stu-id="a49df-107">Member</span></span>|<span data-ttu-id="a49df-108">值</span><span class="sxs-lookup"><span data-stu-id="a49df-108">Value</span></span>|<span data-ttu-id="a49df-109">Description</span><span class="sxs-lookup"><span data-stu-id="a49df-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a49df-110">unknown</span><span class="sxs-lookup"><span data-stu-id="a49df-110">unknown</span></span>|<span data-ttu-id="a49df-111">0</span><span class="sxs-lookup"><span data-stu-id="a49df-111">0</span></span>|<span data-ttu-id="a49df-112">未知。</span><span class="sxs-lookup"><span data-stu-id="a49df-112">Unknown.</span></span>|
|<span data-ttu-id="a49df-113">符合标准</span><span class="sxs-lookup"><span data-stu-id="a49df-113">compliant</span></span>|<span data-ttu-id="a49df-114">1</span><span class="sxs-lookup"><span data-stu-id="a49df-114">1</span></span>|<span data-ttu-id="a49df-115">兼容。</span><span class="sxs-lookup"><span data-stu-id="a49df-115">Compliant.</span></span>|
|<span data-ttu-id="a49df-116">不符合标准</span><span class="sxs-lookup"><span data-stu-id="a49df-116">noncompliant</span></span>|<span data-ttu-id="a49df-117">2</span><span class="sxs-lookup"><span data-stu-id="a49df-117">2</span></span>|<span data-ttu-id="a49df-118">设备不兼容，并阻止从企业资源。</span><span class="sxs-lookup"><span data-stu-id="a49df-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="a49df-119">冲突</span><span class="sxs-lookup"><span data-stu-id="a49df-119">conflict</span></span>|<span data-ttu-id="a49df-120">3</span><span class="sxs-lookup"><span data-stu-id="a49df-120">3</span></span>|<span data-ttu-id="a49df-121">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="a49df-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="a49df-122">error</span><span class="sxs-lookup"><span data-stu-id="a49df-122">error</span></span>|<span data-ttu-id="a49df-123">4</span><span class="sxs-lookup"><span data-stu-id="a49df-123">4</span></span>|<span data-ttu-id="a49df-124">错误。</span><span class="sxs-lookup"><span data-stu-id="a49df-124">Error.</span></span>|
|<span data-ttu-id="a49df-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="a49df-125">inGracePeriod</span></span>|<span data-ttu-id="a49df-126">254</span><span class="sxs-lookup"><span data-stu-id="a49df-126">254</span></span>|<span data-ttu-id="a49df-127">设备不兼容，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="a49df-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="a49df-128">configManager</span><span class="sxs-lookup"><span data-stu-id="a49df-128">configManager</span></span>|<span data-ttu-id="a49df-129">255</span><span class="sxs-lookup"><span data-stu-id="a49df-129">255</span></span>|<span data-ttu-id="a49df-130">配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="a49df-130">Managed by Config Manager</span></span>|



