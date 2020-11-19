---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 50c833bb7ca2067641386bfb0ebfb03394ceba77
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299258"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="75c20-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="75c20-103">deviceManagementExchangeAccessState enum type</span></span>

<span data-ttu-id="75c20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75c20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75c20-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="75c20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75c20-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="75c20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75c20-107">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="75c20-107">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="75c20-108">成员</span><span class="sxs-lookup"><span data-stu-id="75c20-108">Members</span></span>
|<span data-ttu-id="75c20-109">成员</span><span class="sxs-lookup"><span data-stu-id="75c20-109">Member</span></span>|<span data-ttu-id="75c20-110">值</span><span class="sxs-lookup"><span data-stu-id="75c20-110">Value</span></span>|<span data-ttu-id="75c20-111">Description</span><span class="sxs-lookup"><span data-stu-id="75c20-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75c20-112">无</span><span class="sxs-lookup"><span data-stu-id="75c20-112">none</span></span>|<span data-ttu-id="75c20-113">0</span><span class="sxs-lookup"><span data-stu-id="75c20-113">0</span></span>|<span data-ttu-id="75c20-114">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="75c20-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="75c20-115">unknown</span><span class="sxs-lookup"><span data-stu-id="75c20-115">unknown</span></span>|<span data-ttu-id="75c20-116">1</span><span class="sxs-lookup"><span data-stu-id="75c20-116">1</span></span>|<span data-ttu-id="75c20-117">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="75c20-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="75c20-118">支持</span><span class="sxs-lookup"><span data-stu-id="75c20-118">allowed</span></span>|<span data-ttu-id="75c20-119">双面</span><span class="sxs-lookup"><span data-stu-id="75c20-119">2</span></span>|<span data-ttu-id="75c20-120">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="75c20-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="75c20-121">堵塞</span><span class="sxs-lookup"><span data-stu-id="75c20-121">blocked</span></span>|<span data-ttu-id="75c20-122">第三章</span><span class="sxs-lookup"><span data-stu-id="75c20-122">3</span></span>|<span data-ttu-id="75c20-123">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="75c20-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="75c20-124">隔离</span><span class="sxs-lookup"><span data-stu-id="75c20-124">quarantined</span></span>|<span data-ttu-id="75c20-125">4 </span><span class="sxs-lookup"><span data-stu-id="75c20-125">4</span></span>|<span data-ttu-id="75c20-126">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="75c20-126">Device is Quarantined in Exchange</span></span>|




