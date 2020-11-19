---
title: microsoftTunnelServerHealthStatus 枚举类型
description: 可能的 MicrosoftTunnelServer 运行状况类型的枚举
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5c9c00812d0b1e4e3173c981cdaa92c9c0bafec2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301539"
---
# <a name="microsofttunnelserverhealthstatus-enum-type"></a><span data-ttu-id="d60a6-103">microsoftTunnelServerHealthStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d60a6-103">microsoftTunnelServerHealthStatus enum type</span></span>

<span data-ttu-id="d60a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d60a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d60a6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d60a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d60a6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d60a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d60a6-107">可能的 MicrosoftTunnelServer 运行状况类型的枚举</span><span class="sxs-lookup"><span data-stu-id="d60a6-107">Enum of possible MicrosoftTunnelServer health status types</span></span>

## <a name="members"></a><span data-ttu-id="d60a6-108">成员</span><span class="sxs-lookup"><span data-stu-id="d60a6-108">Members</span></span>
|<span data-ttu-id="d60a6-109">成员</span><span class="sxs-lookup"><span data-stu-id="d60a6-109">Member</span></span>|<span data-ttu-id="d60a6-110">值</span><span class="sxs-lookup"><span data-stu-id="d60a6-110">Value</span></span>|<span data-ttu-id="d60a6-111">说明</span><span class="sxs-lookup"><span data-stu-id="d60a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d60a6-112">unknown</span><span class="sxs-lookup"><span data-stu-id="d60a6-112">unknown</span></span>|<span data-ttu-id="d60a6-113">0</span><span class="sxs-lookup"><span data-stu-id="d60a6-113">0</span></span>|<span data-ttu-id="d60a6-114">状态未知</span><span class="sxs-lookup"><span data-stu-id="d60a6-114">The state is unknown</span></span>|
|<span data-ttu-id="d60a6-115">运转</span><span class="sxs-lookup"><span data-stu-id="d60a6-115">healthy</span></span>|<span data-ttu-id="d60a6-116">1</span><span class="sxs-lookup"><span data-stu-id="d60a6-116">1</span></span>|<span data-ttu-id="d60a6-117">状态为 "正常"</span><span class="sxs-lookup"><span data-stu-id="d60a6-117">The state is healthy</span></span>|
|<span data-ttu-id="d60a6-118">正常</span><span class="sxs-lookup"><span data-stu-id="d60a6-118">unhealthy</span></span>|<span data-ttu-id="d60a6-119">双面</span><span class="sxs-lookup"><span data-stu-id="d60a6-119">2</span></span>|<span data-ttu-id="d60a6-120">状态不正常</span><span class="sxs-lookup"><span data-stu-id="d60a6-120">The state is unhealthy</span></span>|
|<span data-ttu-id="d60a6-121">警告</span><span class="sxs-lookup"><span data-stu-id="d60a6-121">warning</span></span>|<span data-ttu-id="d60a6-122">第三章</span><span class="sxs-lookup"><span data-stu-id="d60a6-122">3</span></span>|<span data-ttu-id="d60a6-123">状态为警告</span><span class="sxs-lookup"><span data-stu-id="d60a6-123">The state is warning</span></span>|
|<span data-ttu-id="d60a6-124">脱机</span><span class="sxs-lookup"><span data-stu-id="d60a6-124">offline</span></span>|<span data-ttu-id="d60a6-125">4 </span><span class="sxs-lookup"><span data-stu-id="d60a6-125">4</span></span>|<span data-ttu-id="d60a6-126">状态为脱机</span><span class="sxs-lookup"><span data-stu-id="d60a6-126">The state is offline</span></span>|
|<span data-ttu-id="d60a6-127">upgradeInProgress</span><span class="sxs-lookup"><span data-stu-id="d60a6-127">upgradeInProgress</span></span>|<span data-ttu-id="d60a6-128">5 </span><span class="sxs-lookup"><span data-stu-id="d60a6-128">5</span></span>|<span data-ttu-id="d60a6-129">状态为 upgradeInProgress</span><span class="sxs-lookup"><span data-stu-id="d60a6-129">The state is upgradeInProgress</span></span>|
|<span data-ttu-id="d60a6-130">upgradeFailed</span><span class="sxs-lookup"><span data-stu-id="d60a6-130">upgradeFailed</span></span>|<span data-ttu-id="d60a6-131">6 </span><span class="sxs-lookup"><span data-stu-id="d60a6-131">6</span></span>|<span data-ttu-id="d60a6-132">状态为 upgradeFailed</span><span class="sxs-lookup"><span data-stu-id="d60a6-132">The state is upgradeFailed</span></span>|




