---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fedbd157c4668397256971c57a4cb5fa355f78c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584661"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="b1cc3-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b1cc3-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="b1cc3-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1cc3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1cc3-105">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="b1cc3-105">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="b1cc3-106">成员</span><span class="sxs-lookup"><span data-stu-id="b1cc3-106">Members</span></span>
|<span data-ttu-id="b1cc3-107">成员</span><span class="sxs-lookup"><span data-stu-id="b1cc3-107">Member</span></span>|<span data-ttu-id="b1cc3-108">值</span><span class="sxs-lookup"><span data-stu-id="b1cc3-108">Value</span></span>|<span data-ttu-id="b1cc3-109">说明</span><span class="sxs-lookup"><span data-stu-id="b1cc3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1cc3-110">无</span><span class="sxs-lookup"><span data-stu-id="b1cc3-110">none</span></span>|<span data-ttu-id="b1cc3-111">0</span><span class="sxs-lookup"><span data-stu-id="b1cc3-111">0</span></span>|<span data-ttu-id="b1cc3-112">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1cc3-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="b1cc3-113">unknown</span><span class="sxs-lookup"><span data-stu-id="b1cc3-113">unknown</span></span>|<span data-ttu-id="b1cc3-114">1</span><span class="sxs-lookup"><span data-stu-id="b1cc3-114">1</span></span>|<span data-ttu-id="b1cc3-115">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="b1cc3-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="b1cc3-116">支持</span><span class="sxs-lookup"><span data-stu-id="b1cc3-116">allowed</span></span>|<span data-ttu-id="b1cc3-117">2 </span><span class="sxs-lookup"><span data-stu-id="b1cc3-117">2</span></span>|<span data-ttu-id="b1cc3-118">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="b1cc3-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="b1cc3-119">堵塞</span><span class="sxs-lookup"><span data-stu-id="b1cc3-119">blocked</span></span>|<span data-ttu-id="b1cc3-120">3 </span><span class="sxs-lookup"><span data-stu-id="b1cc3-120">3</span></span>|<span data-ttu-id="b1cc3-121">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="b1cc3-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="b1cc3-122">隔离</span><span class="sxs-lookup"><span data-stu-id="b1cc3-122">quarantined</span></span>|<span data-ttu-id="b1cc3-123">4 </span><span class="sxs-lookup"><span data-stu-id="b1cc3-123">4</span></span>|<span data-ttu-id="b1cc3-124">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="b1cc3-124">Device is Quarantined in Exchange</span></span>|



