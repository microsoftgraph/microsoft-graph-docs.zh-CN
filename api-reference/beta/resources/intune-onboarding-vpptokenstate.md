---
title: vppTokenState 枚举类型
description: 使用 Apple 卷购买计划令牌关联可能的状态。
ms.openlocfilehash: 7180364063a48e1b0eeb2778ed4def7c0d3930a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044711"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="ddfc5-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ddfc5-103">vppTokenState enum type</span></span>

> <span data-ttu-id="ddfc5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ddfc5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddfc5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ddfc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ddfc5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ddfc5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddfc5-107">使用 Apple 卷购买计划令牌关联可能的状态。</span><span class="sxs-lookup"><span data-stu-id="ddfc5-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="ddfc5-108">成员</span><span class="sxs-lookup"><span data-stu-id="ddfc5-108">Members</span></span>
|<span data-ttu-id="ddfc5-109">成员</span><span class="sxs-lookup"><span data-stu-id="ddfc5-109">Member</span></span>|<span data-ttu-id="ddfc5-110">值</span><span class="sxs-lookup"><span data-stu-id="ddfc5-110">Value</span></span>|<span data-ttu-id="ddfc5-111">说明</span><span class="sxs-lookup"><span data-stu-id="ddfc5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddfc5-112">unknown</span><span class="sxs-lookup"><span data-stu-id="ddfc5-112">unknown</span></span>|<span data-ttu-id="ddfc5-113">0</span><span class="sxs-lookup"><span data-stu-id="ddfc5-113">0</span></span>|<span data-ttu-id="ddfc5-114">默认状态。</span><span class="sxs-lookup"><span data-stu-id="ddfc5-114">Default state.</span></span>|
|<span data-ttu-id="ddfc5-115">有效</span><span class="sxs-lookup"><span data-stu-id="ddfc5-115">valid</span></span>|<span data-ttu-id="ddfc5-116">1</span><span class="sxs-lookup"><span data-stu-id="ddfc5-116">1</span></span>|<span data-ttu-id="ddfc5-117">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="ddfc5-117">Token is valid.</span></span>|
|<span data-ttu-id="ddfc5-118">过期</span><span class="sxs-lookup"><span data-stu-id="ddfc5-118">expired</span></span>|<span data-ttu-id="ddfc5-119">2</span><span class="sxs-lookup"><span data-stu-id="ddfc5-119">2</span></span>|<span data-ttu-id="ddfc5-120">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="ddfc5-120">Token is expired.</span></span>|
|<span data-ttu-id="ddfc5-121">无效</span><span class="sxs-lookup"><span data-stu-id="ddfc5-121">invalid</span></span>|<span data-ttu-id="ddfc5-122">3</span><span class="sxs-lookup"><span data-stu-id="ddfc5-122">3</span></span>|<span data-ttu-id="ddfc5-123">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="ddfc5-123">Token is invalid.</span></span>|
|<span data-ttu-id="ddfc5-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="ddfc5-124">assignedToExternalMDM</span></span>|<span data-ttu-id="ddfc5-125">4</span><span class="sxs-lookup"><span data-stu-id="ddfc5-125">4</span></span>|<span data-ttu-id="ddfc5-126">由另一个 MDM 服务管理令牌。</span><span class="sxs-lookup"><span data-stu-id="ddfc5-126">Token is managed by another MDM Service.</span></span>|





