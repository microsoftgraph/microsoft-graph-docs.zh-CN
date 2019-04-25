---
title: vppTokenState 枚举类型
description: 与 Apple volume Purchase Program 令牌关联的可能状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 573fe27064881f670e642e7c3727b8c9eb7db5a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548157"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="cd6ba-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cd6ba-103">vppTokenState enum type</span></span>

> <span data-ttu-id="cd6ba-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd6ba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd6ba-105">与 Apple volume Purchase Program 令牌关联的可能状态。</span><span class="sxs-lookup"><span data-stu-id="cd6ba-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="cd6ba-106">成员</span><span class="sxs-lookup"><span data-stu-id="cd6ba-106">Members</span></span>
|<span data-ttu-id="cd6ba-107">成员</span><span class="sxs-lookup"><span data-stu-id="cd6ba-107">Member</span></span>|<span data-ttu-id="cd6ba-108">值</span><span class="sxs-lookup"><span data-stu-id="cd6ba-108">Value</span></span>|<span data-ttu-id="cd6ba-109">说明</span><span class="sxs-lookup"><span data-stu-id="cd6ba-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd6ba-110">unknown</span><span class="sxs-lookup"><span data-stu-id="cd6ba-110">unknown</span></span>|<span data-ttu-id="cd6ba-111">0</span><span class="sxs-lookup"><span data-stu-id="cd6ba-111">0</span></span>|<span data-ttu-id="cd6ba-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="cd6ba-112">Default state.</span></span>|
|<span data-ttu-id="cd6ba-113">有效</span><span class="sxs-lookup"><span data-stu-id="cd6ba-113">valid</span></span>|<span data-ttu-id="cd6ba-114">1</span><span class="sxs-lookup"><span data-stu-id="cd6ba-114">1</span></span>|<span data-ttu-id="cd6ba-115">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="cd6ba-115">Token is valid.</span></span>|
|<span data-ttu-id="cd6ba-116">期满</span><span class="sxs-lookup"><span data-stu-id="cd6ba-116">expired</span></span>|<span data-ttu-id="cd6ba-117">2 </span><span class="sxs-lookup"><span data-stu-id="cd6ba-117">2</span></span>|<span data-ttu-id="cd6ba-118">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="cd6ba-118">Token is expired.</span></span>|
|<span data-ttu-id="cd6ba-119">无效</span><span class="sxs-lookup"><span data-stu-id="cd6ba-119">invalid</span></span>|<span data-ttu-id="cd6ba-120">3 </span><span class="sxs-lookup"><span data-stu-id="cd6ba-120">3</span></span>|<span data-ttu-id="cd6ba-121">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="cd6ba-121">Token is invalid.</span></span>|
|<span data-ttu-id="cd6ba-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="cd6ba-122">assignedToExternalMDM</span></span>|<span data-ttu-id="cd6ba-123">4 </span><span class="sxs-lookup"><span data-stu-id="cd6ba-123">4</span></span>|<span data-ttu-id="cd6ba-124">令牌由另一个 MDM 服务管理。</span><span class="sxs-lookup"><span data-stu-id="cd6ba-124">Token is managed by another MDM Service.</span></span>|



