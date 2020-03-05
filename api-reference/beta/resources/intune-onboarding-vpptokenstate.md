---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3e78e5762c1d59d882973a44f69482fcb21998f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527690"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="82746-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="82746-103">vppTokenState enum type</span></span>

<span data-ttu-id="82746-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="82746-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82746-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82746-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82746-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82746-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82746-107">与 Apple Volume Purchase Program 令牌关联的可能状态。</span><span class="sxs-lookup"><span data-stu-id="82746-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="82746-108">成员</span><span class="sxs-lookup"><span data-stu-id="82746-108">Members</span></span>
|<span data-ttu-id="82746-109">成员</span><span class="sxs-lookup"><span data-stu-id="82746-109">Member</span></span>|<span data-ttu-id="82746-110">值</span><span class="sxs-lookup"><span data-stu-id="82746-110">Value</span></span>|<span data-ttu-id="82746-111">说明</span><span class="sxs-lookup"><span data-stu-id="82746-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82746-112">unknown</span><span class="sxs-lookup"><span data-stu-id="82746-112">unknown</span></span>|<span data-ttu-id="82746-113">0</span><span class="sxs-lookup"><span data-stu-id="82746-113">0</span></span>|<span data-ttu-id="82746-114">默认状态。</span><span class="sxs-lookup"><span data-stu-id="82746-114">Default state.</span></span>|
|<span data-ttu-id="82746-115">有效</span><span class="sxs-lookup"><span data-stu-id="82746-115">valid</span></span>|<span data-ttu-id="82746-116">1 </span><span class="sxs-lookup"><span data-stu-id="82746-116">1</span></span>|<span data-ttu-id="82746-117">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="82746-117">Token is valid.</span></span>|
|<span data-ttu-id="82746-118">期满</span><span class="sxs-lookup"><span data-stu-id="82746-118">expired</span></span>|<span data-ttu-id="82746-119">2 </span><span class="sxs-lookup"><span data-stu-id="82746-119">2</span></span>|<span data-ttu-id="82746-120">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="82746-120">Token is expired.</span></span>|
|<span data-ttu-id="82746-121">无效</span><span class="sxs-lookup"><span data-stu-id="82746-121">invalid</span></span>|<span data-ttu-id="82746-122">3 </span><span class="sxs-lookup"><span data-stu-id="82746-122">3</span></span>|<span data-ttu-id="82746-123">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="82746-123">Token is invalid.</span></span>|
|<span data-ttu-id="82746-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="82746-124">assignedToExternalMDM</span></span>|<span data-ttu-id="82746-125">4 </span><span class="sxs-lookup"><span data-stu-id="82746-125">4</span></span>|<span data-ttu-id="82746-126">令牌由另一个 MDM 服务管理。</span><span class="sxs-lookup"><span data-stu-id="82746-126">Token is managed by another MDM Service.</span></span>|



