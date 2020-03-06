---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ef97c75379a446c0dc503636e8870dfe14f52ee2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533289"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="afc24-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="afc24-103">deviceManagementExchangeAccessState enum type</span></span>

<span data-ttu-id="afc24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afc24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afc24-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="afc24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afc24-106">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="afc24-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="afc24-107">成员</span><span class="sxs-lookup"><span data-stu-id="afc24-107">Members</span></span>
|<span data-ttu-id="afc24-108">成员</span><span class="sxs-lookup"><span data-stu-id="afc24-108">Member</span></span>|<span data-ttu-id="afc24-109">值</span><span class="sxs-lookup"><span data-stu-id="afc24-109">Value</span></span>|<span data-ttu-id="afc24-110">说明</span><span class="sxs-lookup"><span data-stu-id="afc24-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afc24-111">无</span><span class="sxs-lookup"><span data-stu-id="afc24-111">none</span></span>|<span data-ttu-id="afc24-112">0</span><span class="sxs-lookup"><span data-stu-id="afc24-112">0</span></span>|<span data-ttu-id="afc24-113">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="afc24-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="afc24-114">unknown</span><span class="sxs-lookup"><span data-stu-id="afc24-114">unknown</span></span>|<span data-ttu-id="afc24-115">1 </span><span class="sxs-lookup"><span data-stu-id="afc24-115">1</span></span>|<span data-ttu-id="afc24-116">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="afc24-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="afc24-117">支持</span><span class="sxs-lookup"><span data-stu-id="afc24-117">allowed</span></span>|<span data-ttu-id="afc24-118">2 </span><span class="sxs-lookup"><span data-stu-id="afc24-118">2</span></span>|<span data-ttu-id="afc24-119">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="afc24-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="afc24-120">堵塞</span><span class="sxs-lookup"><span data-stu-id="afc24-120">blocked</span></span>|<span data-ttu-id="afc24-121">3 </span><span class="sxs-lookup"><span data-stu-id="afc24-121">3</span></span>|<span data-ttu-id="afc24-122">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="afc24-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="afc24-123">隔离</span><span class="sxs-lookup"><span data-stu-id="afc24-123">quarantined</span></span>|<span data-ttu-id="afc24-124">4 </span><span class="sxs-lookup"><span data-stu-id="afc24-124">4</span></span>|<span data-ttu-id="afc24-125">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="afc24-125">Device is Quarantined in Exchange</span></span>|




