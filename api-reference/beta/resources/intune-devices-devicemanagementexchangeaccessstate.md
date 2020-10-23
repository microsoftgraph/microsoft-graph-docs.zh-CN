---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2333cb2165971c6a30a85d19d21184cb9c40aa53
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693708"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="dcb2c-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dcb2c-103">deviceManagementExchangeAccessState enum type</span></span>

<span data-ttu-id="dcb2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcb2c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcb2c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dcb2c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcb2c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dcb2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcb2c-107">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="dcb2c-107">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="dcb2c-108">成员</span><span class="sxs-lookup"><span data-stu-id="dcb2c-108">Members</span></span>
|<span data-ttu-id="dcb2c-109">成员</span><span class="sxs-lookup"><span data-stu-id="dcb2c-109">Member</span></span>|<span data-ttu-id="dcb2c-110">值</span><span class="sxs-lookup"><span data-stu-id="dcb2c-110">Value</span></span>|<span data-ttu-id="dcb2c-111">说明</span><span class="sxs-lookup"><span data-stu-id="dcb2c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcb2c-112">无</span><span class="sxs-lookup"><span data-stu-id="dcb2c-112">none</span></span>|<span data-ttu-id="dcb2c-113">0</span><span class="sxs-lookup"><span data-stu-id="dcb2c-113">0</span></span>|<span data-ttu-id="dcb2c-114">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="dcb2c-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="dcb2c-115">unknown</span><span class="sxs-lookup"><span data-stu-id="dcb2c-115">unknown</span></span>|<span data-ttu-id="dcb2c-116">1</span><span class="sxs-lookup"><span data-stu-id="dcb2c-116">1</span></span>|<span data-ttu-id="dcb2c-117">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="dcb2c-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="dcb2c-118">支持</span><span class="sxs-lookup"><span data-stu-id="dcb2c-118">allowed</span></span>|<span data-ttu-id="dcb2c-119">双面</span><span class="sxs-lookup"><span data-stu-id="dcb2c-119">2</span></span>|<span data-ttu-id="dcb2c-120">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="dcb2c-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="dcb2c-121">堵塞</span><span class="sxs-lookup"><span data-stu-id="dcb2c-121">blocked</span></span>|<span data-ttu-id="dcb2c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="dcb2c-122">3</span></span>|<span data-ttu-id="dcb2c-123">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="dcb2c-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="dcb2c-124">隔离</span><span class="sxs-lookup"><span data-stu-id="dcb2c-124">quarantined</span></span>|<span data-ttu-id="dcb2c-125">4 </span><span class="sxs-lookup"><span data-stu-id="dcb2c-125">4</span></span>|<span data-ttu-id="dcb2c-126">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="dcb2c-126">Device is Quarantined in Exchange</span></span>|





