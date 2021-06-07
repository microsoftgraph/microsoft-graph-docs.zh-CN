---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 26492a317a5fe147a49cc8cda7103fa492704deb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755698"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="7a0b7-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7a0b7-103">vppTokenState enum type</span></span>

<span data-ttu-id="7a0b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a0b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a0b7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a0b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a0b7-106">与 Apple Volume Purchase Program 令牌关联的可能状态。</span><span class="sxs-lookup"><span data-stu-id="7a0b7-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="7a0b7-107">成员</span><span class="sxs-lookup"><span data-stu-id="7a0b7-107">Members</span></span>
|<span data-ttu-id="7a0b7-108">成员</span><span class="sxs-lookup"><span data-stu-id="7a0b7-108">Member</span></span>|<span data-ttu-id="7a0b7-109">值</span><span class="sxs-lookup"><span data-stu-id="7a0b7-109">Value</span></span>|<span data-ttu-id="7a0b7-110">Description</span><span class="sxs-lookup"><span data-stu-id="7a0b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a0b7-111">unknown</span><span class="sxs-lookup"><span data-stu-id="7a0b7-111">unknown</span></span>|<span data-ttu-id="7a0b7-112">0</span><span class="sxs-lookup"><span data-stu-id="7a0b7-112">0</span></span>|<span data-ttu-id="7a0b7-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="7a0b7-113">Default state.</span></span>|
|<span data-ttu-id="7a0b7-114">valid</span><span class="sxs-lookup"><span data-stu-id="7a0b7-114">valid</span></span>|<span data-ttu-id="7a0b7-115">1</span><span class="sxs-lookup"><span data-stu-id="7a0b7-115">1</span></span>|<span data-ttu-id="7a0b7-116">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="7a0b7-116">Token is valid.</span></span>|
|<span data-ttu-id="7a0b7-117">已过期</span><span class="sxs-lookup"><span data-stu-id="7a0b7-117">expired</span></span>|<span data-ttu-id="7a0b7-118">2</span><span class="sxs-lookup"><span data-stu-id="7a0b7-118">2</span></span>|<span data-ttu-id="7a0b7-119">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="7a0b7-119">Token is expired.</span></span>|
|<span data-ttu-id="7a0b7-120">无效</span><span class="sxs-lookup"><span data-stu-id="7a0b7-120">invalid</span></span>|<span data-ttu-id="7a0b7-121">3</span><span class="sxs-lookup"><span data-stu-id="7a0b7-121">3</span></span>|<span data-ttu-id="7a0b7-122">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="7a0b7-122">Token is invalid.</span></span>|
|<span data-ttu-id="7a0b7-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="7a0b7-123">assignedToExternalMDM</span></span>|<span data-ttu-id="7a0b7-124">4 </span><span class="sxs-lookup"><span data-stu-id="7a0b7-124">4</span></span>|<span data-ttu-id="7a0b7-125">令牌由另一个 MDM 服务管理。</span><span class="sxs-lookup"><span data-stu-id="7a0b7-125">Token is managed by another MDM Service.</span></span>|




