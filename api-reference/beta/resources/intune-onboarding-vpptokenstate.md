---
title: vppTokenState 枚举类型
description: 使用 Apple 卷购买计划令牌关联可能的状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7d0c4ee7ae0b8e35f97a18d0958a2456cab40a10
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416158"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="21ea8-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="21ea8-103">vppTokenState enum type</span></span>

> <span data-ttu-id="21ea8-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="21ea8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="21ea8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="21ea8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21ea8-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21ea8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21ea8-107">使用 Apple 卷购买计划令牌关联可能的状态。</span><span class="sxs-lookup"><span data-stu-id="21ea8-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="21ea8-108">成员</span><span class="sxs-lookup"><span data-stu-id="21ea8-108">Members</span></span>
|<span data-ttu-id="21ea8-109">成员</span><span class="sxs-lookup"><span data-stu-id="21ea8-109">Member</span></span>|<span data-ttu-id="21ea8-110">值</span><span class="sxs-lookup"><span data-stu-id="21ea8-110">Value</span></span>|<span data-ttu-id="21ea8-111">说明</span><span class="sxs-lookup"><span data-stu-id="21ea8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21ea8-112">unknown</span><span class="sxs-lookup"><span data-stu-id="21ea8-112">unknown</span></span>|<span data-ttu-id="21ea8-113">0</span><span class="sxs-lookup"><span data-stu-id="21ea8-113">0</span></span>|<span data-ttu-id="21ea8-114">默认状态。</span><span class="sxs-lookup"><span data-stu-id="21ea8-114">Default state.</span></span>|
|<span data-ttu-id="21ea8-115">有效</span><span class="sxs-lookup"><span data-stu-id="21ea8-115">valid</span></span>|<span data-ttu-id="21ea8-116">1</span><span class="sxs-lookup"><span data-stu-id="21ea8-116">1</span></span>|<span data-ttu-id="21ea8-117">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="21ea8-117">Token is valid.</span></span>|
|<span data-ttu-id="21ea8-118">过期</span><span class="sxs-lookup"><span data-stu-id="21ea8-118">expired</span></span>|<span data-ttu-id="21ea8-119">2</span><span class="sxs-lookup"><span data-stu-id="21ea8-119">2</span></span>|<span data-ttu-id="21ea8-120">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="21ea8-120">Token is expired.</span></span>|
|<span data-ttu-id="21ea8-121">无效</span><span class="sxs-lookup"><span data-stu-id="21ea8-121">invalid</span></span>|<span data-ttu-id="21ea8-122">3</span><span class="sxs-lookup"><span data-stu-id="21ea8-122">3</span></span>|<span data-ttu-id="21ea8-123">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="21ea8-123">Token is invalid.</span></span>|
|<span data-ttu-id="21ea8-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="21ea8-124">assignedToExternalMDM</span></span>|<span data-ttu-id="21ea8-125">4</span><span class="sxs-lookup"><span data-stu-id="21ea8-125">4</span></span>|<span data-ttu-id="21ea8-126">由另一个 MDM 服务管理令牌。</span><span class="sxs-lookup"><span data-stu-id="21ea8-126">Token is managed by another MDM Service.</span></span>|




