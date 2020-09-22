---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4e59dea6ba916745e8e9e0bc58ab20ba637e9ba5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091185"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="75bde-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="75bde-103">deviceManagementExchangeAccessState enum type</span></span>

<span data-ttu-id="75bde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75bde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75bde-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="75bde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75bde-106">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="75bde-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="75bde-107">成员</span><span class="sxs-lookup"><span data-stu-id="75bde-107">Members</span></span>
|<span data-ttu-id="75bde-108">成员</span><span class="sxs-lookup"><span data-stu-id="75bde-108">Member</span></span>|<span data-ttu-id="75bde-109">值</span><span class="sxs-lookup"><span data-stu-id="75bde-109">Value</span></span>|<span data-ttu-id="75bde-110">说明</span><span class="sxs-lookup"><span data-stu-id="75bde-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75bde-111">无</span><span class="sxs-lookup"><span data-stu-id="75bde-111">none</span></span>|<span data-ttu-id="75bde-112">0</span><span class="sxs-lookup"><span data-stu-id="75bde-112">0</span></span>|<span data-ttu-id="75bde-113">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="75bde-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="75bde-114">unknown</span><span class="sxs-lookup"><span data-stu-id="75bde-114">unknown</span></span>|<span data-ttu-id="75bde-115">1 </span><span class="sxs-lookup"><span data-stu-id="75bde-115">1</span></span>|<span data-ttu-id="75bde-116">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="75bde-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="75bde-117">支持</span><span class="sxs-lookup"><span data-stu-id="75bde-117">allowed</span></span>|<span data-ttu-id="75bde-118">2 </span><span class="sxs-lookup"><span data-stu-id="75bde-118">2</span></span>|<span data-ttu-id="75bde-119">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="75bde-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="75bde-120">堵塞</span><span class="sxs-lookup"><span data-stu-id="75bde-120">blocked</span></span>|<span data-ttu-id="75bde-121">第三章</span><span class="sxs-lookup"><span data-stu-id="75bde-121">3</span></span>|<span data-ttu-id="75bde-122">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="75bde-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="75bde-123">隔离</span><span class="sxs-lookup"><span data-stu-id="75bde-123">quarantined</span></span>|<span data-ttu-id="75bde-124">4 </span><span class="sxs-lookup"><span data-stu-id="75bde-124">4</span></span>|<span data-ttu-id="75bde-125">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="75bde-125">Device is Quarantined in Exchange</span></span>|









