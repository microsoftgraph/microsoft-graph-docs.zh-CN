---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 15b0dd7b99d8395b7c66171969bad1cb79bce0b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159582"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="ba479-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ba479-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="ba479-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ba479-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba479-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba479-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba479-106">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="ba479-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="ba479-107">成员</span><span class="sxs-lookup"><span data-stu-id="ba479-107">Members</span></span>
|<span data-ttu-id="ba479-108">成员</span><span class="sxs-lookup"><span data-stu-id="ba479-108">Member</span></span>|<span data-ttu-id="ba479-109">值</span><span class="sxs-lookup"><span data-stu-id="ba479-109">Value</span></span>|<span data-ttu-id="ba479-110">说明</span><span class="sxs-lookup"><span data-stu-id="ba479-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba479-111">无</span><span class="sxs-lookup"><span data-stu-id="ba479-111">none</span></span>|<span data-ttu-id="ba479-112">0</span><span class="sxs-lookup"><span data-stu-id="ba479-112">0</span></span>|<span data-ttu-id="ba479-113">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="ba479-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="ba479-114">unknown</span><span class="sxs-lookup"><span data-stu-id="ba479-114">unknown</span></span>|<span data-ttu-id="ba479-115">1</span><span class="sxs-lookup"><span data-stu-id="ba479-115">1</span></span>|<span data-ttu-id="ba479-116">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="ba479-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="ba479-117">支持</span><span class="sxs-lookup"><span data-stu-id="ba479-117">allowed</span></span>|<span data-ttu-id="ba479-118">双面</span><span class="sxs-lookup"><span data-stu-id="ba479-118">2</span></span>|<span data-ttu-id="ba479-119">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="ba479-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="ba479-120">已阻止</span><span class="sxs-lookup"><span data-stu-id="ba479-120">blocked</span></span>|<span data-ttu-id="ba479-121">第三章</span><span class="sxs-lookup"><span data-stu-id="ba479-121">3</span></span>|<span data-ttu-id="ba479-122">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="ba479-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="ba479-123">隔离</span><span class="sxs-lookup"><span data-stu-id="ba479-123">quarantined</span></span>|<span data-ttu-id="ba479-124">4</span><span class="sxs-lookup"><span data-stu-id="ba479-124">4</span></span>|<span data-ttu-id="ba479-125">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="ba479-125">Device is Quarantined in Exchange</span></span>|




