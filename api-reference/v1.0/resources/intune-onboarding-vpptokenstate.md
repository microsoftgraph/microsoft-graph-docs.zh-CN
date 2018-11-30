---
title: vppTokenState 枚举类型
description: 使用 Apple 卷购买计划令牌关联可能的状态。
ms.openlocfilehash: 74d7ea2e0ca2dd03b82b71bea2ab5300214b095d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007882"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="29f7e-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="29f7e-103">vppTokenState enum type</span></span>

> <span data-ttu-id="29f7e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="29f7e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29f7e-105">使用 Apple 卷购买计划令牌关联可能的状态。</span><span class="sxs-lookup"><span data-stu-id="29f7e-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="29f7e-106">成员</span><span class="sxs-lookup"><span data-stu-id="29f7e-106">Members</span></span>
|<span data-ttu-id="29f7e-107">成员</span><span class="sxs-lookup"><span data-stu-id="29f7e-107">Member</span></span>|<span data-ttu-id="29f7e-108">值</span><span class="sxs-lookup"><span data-stu-id="29f7e-108">Value</span></span>|<span data-ttu-id="29f7e-109">说明</span><span class="sxs-lookup"><span data-stu-id="29f7e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29f7e-110">unknown</span><span class="sxs-lookup"><span data-stu-id="29f7e-110">unknown</span></span>|<span data-ttu-id="29f7e-111">0</span><span class="sxs-lookup"><span data-stu-id="29f7e-111">0</span></span>|<span data-ttu-id="29f7e-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="29f7e-112">Default state.</span></span>|
|<span data-ttu-id="29f7e-113">有效</span><span class="sxs-lookup"><span data-stu-id="29f7e-113">valid</span></span>|<span data-ttu-id="29f7e-114">1</span><span class="sxs-lookup"><span data-stu-id="29f7e-114">1</span></span>|<span data-ttu-id="29f7e-115">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="29f7e-115">Token is valid.</span></span>|
|<span data-ttu-id="29f7e-116">过期</span><span class="sxs-lookup"><span data-stu-id="29f7e-116">expired</span></span>|<span data-ttu-id="29f7e-117">2</span><span class="sxs-lookup"><span data-stu-id="29f7e-117">2</span></span>|<span data-ttu-id="29f7e-118">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="29f7e-118">Token is expired.</span></span>|
|<span data-ttu-id="29f7e-119">无效</span><span class="sxs-lookup"><span data-stu-id="29f7e-119">invalid</span></span>|<span data-ttu-id="29f7e-120">3</span><span class="sxs-lookup"><span data-stu-id="29f7e-120">3</span></span>|<span data-ttu-id="29f7e-121">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="29f7e-121">Token is invalid.</span></span>|
|<span data-ttu-id="29f7e-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="29f7e-122">assignedToExternalMDM</span></span>|<span data-ttu-id="29f7e-123">4</span><span class="sxs-lookup"><span data-stu-id="29f7e-123">4</span></span>|<span data-ttu-id="29f7e-124">由另一个 MDM 服务管理令牌。</span><span class="sxs-lookup"><span data-stu-id="29f7e-124">Token is managed by another MDM Service.</span></span>|



