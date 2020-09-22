---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 07a9441923e99089fc3dc2ebe9627972237207e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025275"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="c05af-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c05af-103">vppTokenState enum type</span></span>

<span data-ttu-id="c05af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c05af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c05af-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c05af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c05af-106">与 Apple Volume Purchase Program 令牌关联的可能状态。</span><span class="sxs-lookup"><span data-stu-id="c05af-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="c05af-107">成员</span><span class="sxs-lookup"><span data-stu-id="c05af-107">Members</span></span>
|<span data-ttu-id="c05af-108">成员</span><span class="sxs-lookup"><span data-stu-id="c05af-108">Member</span></span>|<span data-ttu-id="c05af-109">值</span><span class="sxs-lookup"><span data-stu-id="c05af-109">Value</span></span>|<span data-ttu-id="c05af-110">说明</span><span class="sxs-lookup"><span data-stu-id="c05af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c05af-111">unknown</span><span class="sxs-lookup"><span data-stu-id="c05af-111">unknown</span></span>|<span data-ttu-id="c05af-112">0</span><span class="sxs-lookup"><span data-stu-id="c05af-112">0</span></span>|<span data-ttu-id="c05af-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="c05af-113">Default state.</span></span>|
|<span data-ttu-id="c05af-114">有效</span><span class="sxs-lookup"><span data-stu-id="c05af-114">valid</span></span>|<span data-ttu-id="c05af-115">1 </span><span class="sxs-lookup"><span data-stu-id="c05af-115">1</span></span>|<span data-ttu-id="c05af-116">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="c05af-116">Token is valid.</span></span>|
|<span data-ttu-id="c05af-117">期满</span><span class="sxs-lookup"><span data-stu-id="c05af-117">expired</span></span>|<span data-ttu-id="c05af-118">2 </span><span class="sxs-lookup"><span data-stu-id="c05af-118">2</span></span>|<span data-ttu-id="c05af-119">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="c05af-119">Token is expired.</span></span>|
|<span data-ttu-id="c05af-120">无效</span><span class="sxs-lookup"><span data-stu-id="c05af-120">invalid</span></span>|<span data-ttu-id="c05af-121">第三章</span><span class="sxs-lookup"><span data-stu-id="c05af-121">3</span></span>|<span data-ttu-id="c05af-122">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="c05af-122">Token is invalid.</span></span>|
|<span data-ttu-id="c05af-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="c05af-123">assignedToExternalMDM</span></span>|<span data-ttu-id="c05af-124">4 </span><span class="sxs-lookup"><span data-stu-id="c05af-124">4</span></span>|<span data-ttu-id="c05af-125">令牌由另一个 MDM 服务管理。</span><span class="sxs-lookup"><span data-stu-id="c05af-125">Token is managed by another MDM Service.</span></span>|









