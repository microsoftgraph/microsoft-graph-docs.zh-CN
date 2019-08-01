---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5969c28aab1b54d8922c6391cf994274ef3570a0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030819"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="8e506-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8e506-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="8e506-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e506-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e506-105">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="8e506-105">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="8e506-106">成员</span><span class="sxs-lookup"><span data-stu-id="8e506-106">Members</span></span>
|<span data-ttu-id="8e506-107">成员</span><span class="sxs-lookup"><span data-stu-id="8e506-107">Member</span></span>|<span data-ttu-id="8e506-108">值</span><span class="sxs-lookup"><span data-stu-id="8e506-108">Value</span></span>|<span data-ttu-id="8e506-109">说明</span><span class="sxs-lookup"><span data-stu-id="8e506-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e506-110">无</span><span class="sxs-lookup"><span data-stu-id="8e506-110">none</span></span>|<span data-ttu-id="8e506-111">0</span><span class="sxs-lookup"><span data-stu-id="8e506-111">0</span></span>|<span data-ttu-id="8e506-112">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="8e506-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="8e506-113">unknown</span><span class="sxs-lookup"><span data-stu-id="8e506-113">unknown</span></span>|<span data-ttu-id="8e506-114">1</span><span class="sxs-lookup"><span data-stu-id="8e506-114">1</span></span>|<span data-ttu-id="8e506-115">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="8e506-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="8e506-116">支持</span><span class="sxs-lookup"><span data-stu-id="8e506-116">allowed</span></span>|<span data-ttu-id="8e506-117">双面</span><span class="sxs-lookup"><span data-stu-id="8e506-117">2</span></span>|<span data-ttu-id="8e506-118">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="8e506-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="8e506-119">堵塞</span><span class="sxs-lookup"><span data-stu-id="8e506-119">blocked</span></span>|<span data-ttu-id="8e506-120">第三章</span><span class="sxs-lookup"><span data-stu-id="8e506-120">3</span></span>|<span data-ttu-id="8e506-121">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="8e506-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="8e506-122">隔离</span><span class="sxs-lookup"><span data-stu-id="8e506-122">quarantined</span></span>|<span data-ttu-id="8e506-123">4</span><span class="sxs-lookup"><span data-stu-id="8e506-123">4</span></span>|<span data-ttu-id="8e506-124">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="8e506-124">Device is Quarantined in Exchange</span></span>|



