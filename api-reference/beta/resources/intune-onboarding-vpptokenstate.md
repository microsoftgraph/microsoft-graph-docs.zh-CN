---
title: vppTokenState 枚举类型
description: 使用 Apple 卷购买计划令牌关联可能的状态。
author: tfitzmac
ms.openlocfilehash: 70ff74a888e351d7f55c64a68771e221f9a644b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306578"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="4c687-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4c687-103">vppTokenState enum type</span></span>

> <span data-ttu-id="4c687-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4c687-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c687-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4c687-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c687-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4c687-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c687-107">使用 Apple 卷购买计划令牌关联可能的状态。</span><span class="sxs-lookup"><span data-stu-id="4c687-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="4c687-108">成员</span><span class="sxs-lookup"><span data-stu-id="4c687-108">Members</span></span>
|<span data-ttu-id="4c687-109">成员</span><span class="sxs-lookup"><span data-stu-id="4c687-109">Member</span></span>|<span data-ttu-id="4c687-110">值</span><span class="sxs-lookup"><span data-stu-id="4c687-110">Value</span></span>|<span data-ttu-id="4c687-111">说明</span><span class="sxs-lookup"><span data-stu-id="4c687-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c687-112">unknown</span><span class="sxs-lookup"><span data-stu-id="4c687-112">unknown</span></span>|<span data-ttu-id="4c687-113">0</span><span class="sxs-lookup"><span data-stu-id="4c687-113">0</span></span>|<span data-ttu-id="4c687-114">默认状态。</span><span class="sxs-lookup"><span data-stu-id="4c687-114">Default state.</span></span>|
|<span data-ttu-id="4c687-115">有效</span><span class="sxs-lookup"><span data-stu-id="4c687-115">valid</span></span>|<span data-ttu-id="4c687-116">1</span><span class="sxs-lookup"><span data-stu-id="4c687-116">1</span></span>|<span data-ttu-id="4c687-117">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="4c687-117">Token is valid.</span></span>|
|<span data-ttu-id="4c687-118">过期</span><span class="sxs-lookup"><span data-stu-id="4c687-118">expired</span></span>|<span data-ttu-id="4c687-119">2</span><span class="sxs-lookup"><span data-stu-id="4c687-119">2</span></span>|<span data-ttu-id="4c687-120">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="4c687-120">Token is expired.</span></span>|
|<span data-ttu-id="4c687-121">无效</span><span class="sxs-lookup"><span data-stu-id="4c687-121">invalid</span></span>|<span data-ttu-id="4c687-122">3</span><span class="sxs-lookup"><span data-stu-id="4c687-122">3</span></span>|<span data-ttu-id="4c687-123">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="4c687-123">Token is invalid.</span></span>|
|<span data-ttu-id="4c687-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="4c687-124">assignedToExternalMDM</span></span>|<span data-ttu-id="4c687-125">4</span><span class="sxs-lookup"><span data-stu-id="4c687-125">4</span></span>|<span data-ttu-id="4c687-126">由另一个 MDM 服务管理令牌。</span><span class="sxs-lookup"><span data-stu-id="4c687-126">Token is managed by another MDM Service.</span></span>|





