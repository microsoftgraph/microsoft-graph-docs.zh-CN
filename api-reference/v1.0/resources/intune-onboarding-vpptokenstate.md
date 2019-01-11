---
title: vppTokenState 枚举类型
description: 使用 Apple 卷购买计划令牌关联可能的状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 89d28a07bb2c6abea2e2a10d9b5a0961e5efecff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834023"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="2bebb-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2bebb-103">vppTokenState enum type</span></span>

> <span data-ttu-id="2bebb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2bebb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2bebb-105">使用 Apple 卷购买计划令牌关联可能的状态。</span><span class="sxs-lookup"><span data-stu-id="2bebb-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="2bebb-106">成员</span><span class="sxs-lookup"><span data-stu-id="2bebb-106">Members</span></span>
|<span data-ttu-id="2bebb-107">成员</span><span class="sxs-lookup"><span data-stu-id="2bebb-107">Member</span></span>|<span data-ttu-id="2bebb-108">值</span><span class="sxs-lookup"><span data-stu-id="2bebb-108">Value</span></span>|<span data-ttu-id="2bebb-109">Description</span><span class="sxs-lookup"><span data-stu-id="2bebb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bebb-110">unknown</span><span class="sxs-lookup"><span data-stu-id="2bebb-110">unknown</span></span>|<span data-ttu-id="2bebb-111">0</span><span class="sxs-lookup"><span data-stu-id="2bebb-111">0</span></span>|<span data-ttu-id="2bebb-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="2bebb-112">Default state.</span></span>|
|<span data-ttu-id="2bebb-113">有效</span><span class="sxs-lookup"><span data-stu-id="2bebb-113">valid</span></span>|<span data-ttu-id="2bebb-114">1</span><span class="sxs-lookup"><span data-stu-id="2bebb-114">1</span></span>|<span data-ttu-id="2bebb-115">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="2bebb-115">Token is valid.</span></span>|
|<span data-ttu-id="2bebb-116">过期</span><span class="sxs-lookup"><span data-stu-id="2bebb-116">expired</span></span>|<span data-ttu-id="2bebb-117">2</span><span class="sxs-lookup"><span data-stu-id="2bebb-117">2</span></span>|<span data-ttu-id="2bebb-118">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="2bebb-118">Token is expired.</span></span>|
|<span data-ttu-id="2bebb-119">无效</span><span class="sxs-lookup"><span data-stu-id="2bebb-119">invalid</span></span>|<span data-ttu-id="2bebb-120">3</span><span class="sxs-lookup"><span data-stu-id="2bebb-120">3</span></span>|<span data-ttu-id="2bebb-121">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="2bebb-121">Token is invalid.</span></span>|
|<span data-ttu-id="2bebb-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="2bebb-122">assignedToExternalMDM</span></span>|<span data-ttu-id="2bebb-123">4</span><span class="sxs-lookup"><span data-stu-id="2bebb-123">4</span></span>|<span data-ttu-id="2bebb-124">由另一个 MDM 服务管理令牌。</span><span class="sxs-lookup"><span data-stu-id="2bebb-124">Token is managed by another MDM Service.</span></span>|



