---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ddc44952bb69288f70fb368309eaf2ef1bfe8f49
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784928"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="e194d-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e194d-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="e194d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e194d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e194d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e194d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e194d-106">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="e194d-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="e194d-107">成员</span><span class="sxs-lookup"><span data-stu-id="e194d-107">Members</span></span>
|<span data-ttu-id="e194d-108">成员</span><span class="sxs-lookup"><span data-stu-id="e194d-108">Member</span></span>|<span data-ttu-id="e194d-109">值</span><span class="sxs-lookup"><span data-stu-id="e194d-109">Value</span></span>|<span data-ttu-id="e194d-110">说明</span><span class="sxs-lookup"><span data-stu-id="e194d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e194d-111">无</span><span class="sxs-lookup"><span data-stu-id="e194d-111">none</span></span>|<span data-ttu-id="e194d-112">0</span><span class="sxs-lookup"><span data-stu-id="e194d-112">0</span></span>|<span data-ttu-id="e194d-113">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="e194d-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="e194d-114">unknown</span><span class="sxs-lookup"><span data-stu-id="e194d-114">unknown</span></span>|<span data-ttu-id="e194d-115">1</span><span class="sxs-lookup"><span data-stu-id="e194d-115">1</span></span>|<span data-ttu-id="e194d-116">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="e194d-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="e194d-117">支持</span><span class="sxs-lookup"><span data-stu-id="e194d-117">allowed</span></span>|<span data-ttu-id="e194d-118">双面</span><span class="sxs-lookup"><span data-stu-id="e194d-118">2</span></span>|<span data-ttu-id="e194d-119">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="e194d-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="e194d-120">堵塞</span><span class="sxs-lookup"><span data-stu-id="e194d-120">blocked</span></span>|<span data-ttu-id="e194d-121">第三章</span><span class="sxs-lookup"><span data-stu-id="e194d-121">3</span></span>|<span data-ttu-id="e194d-122">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="e194d-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="e194d-123">隔离</span><span class="sxs-lookup"><span data-stu-id="e194d-123">quarantined</span></span>|<span data-ttu-id="e194d-124">4 </span><span class="sxs-lookup"><span data-stu-id="e194d-124">4</span></span>|<span data-ttu-id="e194d-125">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="e194d-125">Device is Quarantined in Exchange</span></span>|



