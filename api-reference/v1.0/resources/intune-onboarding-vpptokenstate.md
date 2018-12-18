---
title: vppTokenState 枚举类型
description: 使用 Apple 卷购买计划令牌关联可能的状态。
author: tfitzmac
ms.openlocfilehash: e034f9712e2ef40b40b209935ed96f07b35cdbb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321180"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="1ed3f-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1ed3f-103">vppTokenState enum type</span></span>

> <span data-ttu-id="1ed3f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1ed3f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ed3f-105">使用 Apple 卷购买计划令牌关联可能的状态。</span><span class="sxs-lookup"><span data-stu-id="1ed3f-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="1ed3f-106">成员</span><span class="sxs-lookup"><span data-stu-id="1ed3f-106">Members</span></span>
|<span data-ttu-id="1ed3f-107">成员</span><span class="sxs-lookup"><span data-stu-id="1ed3f-107">Member</span></span>|<span data-ttu-id="1ed3f-108">值</span><span class="sxs-lookup"><span data-stu-id="1ed3f-108">Value</span></span>|<span data-ttu-id="1ed3f-109">说明</span><span class="sxs-lookup"><span data-stu-id="1ed3f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ed3f-110">unknown</span><span class="sxs-lookup"><span data-stu-id="1ed3f-110">unknown</span></span>|<span data-ttu-id="1ed3f-111">0</span><span class="sxs-lookup"><span data-stu-id="1ed3f-111">0</span></span>|<span data-ttu-id="1ed3f-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="1ed3f-112">Default state.</span></span>|
|<span data-ttu-id="1ed3f-113">有效</span><span class="sxs-lookup"><span data-stu-id="1ed3f-113">valid</span></span>|<span data-ttu-id="1ed3f-114">1</span><span class="sxs-lookup"><span data-stu-id="1ed3f-114">1</span></span>|<span data-ttu-id="1ed3f-115">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="1ed3f-115">Token is valid.</span></span>|
|<span data-ttu-id="1ed3f-116">过期</span><span class="sxs-lookup"><span data-stu-id="1ed3f-116">expired</span></span>|<span data-ttu-id="1ed3f-117">2</span><span class="sxs-lookup"><span data-stu-id="1ed3f-117">2</span></span>|<span data-ttu-id="1ed3f-118">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="1ed3f-118">Token is expired.</span></span>|
|<span data-ttu-id="1ed3f-119">无效</span><span class="sxs-lookup"><span data-stu-id="1ed3f-119">invalid</span></span>|<span data-ttu-id="1ed3f-120">3</span><span class="sxs-lookup"><span data-stu-id="1ed3f-120">3</span></span>|<span data-ttu-id="1ed3f-121">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="1ed3f-121">Token is invalid.</span></span>|
|<span data-ttu-id="1ed3f-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="1ed3f-122">assignedToExternalMDM</span></span>|<span data-ttu-id="1ed3f-123">4</span><span class="sxs-lookup"><span data-stu-id="1ed3f-123">4</span></span>|<span data-ttu-id="1ed3f-124">由另一个 MDM 服务管理令牌。</span><span class="sxs-lookup"><span data-stu-id="1ed3f-124">Token is managed by another MDM Service.</span></span>|



