---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fb7f674a458028ba6e90e608086d425fa0538aff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525073"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="b9de8-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b9de8-103">deviceManagementExchangeAccessState enum type</span></span>

<span data-ttu-id="b9de8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b9de8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9de8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9de8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9de8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9de8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9de8-107">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="b9de8-107">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="b9de8-108">成员</span><span class="sxs-lookup"><span data-stu-id="b9de8-108">Members</span></span>
|<span data-ttu-id="b9de8-109">成员</span><span class="sxs-lookup"><span data-stu-id="b9de8-109">Member</span></span>|<span data-ttu-id="b9de8-110">值</span><span class="sxs-lookup"><span data-stu-id="b9de8-110">Value</span></span>|<span data-ttu-id="b9de8-111">说明</span><span class="sxs-lookup"><span data-stu-id="b9de8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9de8-112">无</span><span class="sxs-lookup"><span data-stu-id="b9de8-112">none</span></span>|<span data-ttu-id="b9de8-113">0</span><span class="sxs-lookup"><span data-stu-id="b9de8-113">0</span></span>|<span data-ttu-id="b9de8-114">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="b9de8-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="b9de8-115">unknown</span><span class="sxs-lookup"><span data-stu-id="b9de8-115">unknown</span></span>|<span data-ttu-id="b9de8-116">1 </span><span class="sxs-lookup"><span data-stu-id="b9de8-116">1</span></span>|<span data-ttu-id="b9de8-117">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="b9de8-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="b9de8-118">支持</span><span class="sxs-lookup"><span data-stu-id="b9de8-118">allowed</span></span>|<span data-ttu-id="b9de8-119">2 </span><span class="sxs-lookup"><span data-stu-id="b9de8-119">2</span></span>|<span data-ttu-id="b9de8-120">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="b9de8-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="b9de8-121">堵塞</span><span class="sxs-lookup"><span data-stu-id="b9de8-121">blocked</span></span>|<span data-ttu-id="b9de8-122">3 </span><span class="sxs-lookup"><span data-stu-id="b9de8-122">3</span></span>|<span data-ttu-id="b9de8-123">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="b9de8-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="b9de8-124">隔离</span><span class="sxs-lookup"><span data-stu-id="b9de8-124">quarantined</span></span>|<span data-ttu-id="b9de8-125">4 </span><span class="sxs-lookup"><span data-stu-id="b9de8-125">4</span></span>|<span data-ttu-id="b9de8-126">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="b9de8-126">Device is Quarantined in Exchange</span></span>|



