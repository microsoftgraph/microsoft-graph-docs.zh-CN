---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 26f75ccd2957d7cc9db9b05bb48f4a9eacc36a17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999897"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="89ba7-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="89ba7-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="89ba7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89ba7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89ba7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89ba7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89ba7-106">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="89ba7-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="89ba7-107">成员</span><span class="sxs-lookup"><span data-stu-id="89ba7-107">Members</span></span>
|<span data-ttu-id="89ba7-108">成员</span><span class="sxs-lookup"><span data-stu-id="89ba7-108">Member</span></span>|<span data-ttu-id="89ba7-109">值</span><span class="sxs-lookup"><span data-stu-id="89ba7-109">Value</span></span>|<span data-ttu-id="89ba7-110">说明</span><span class="sxs-lookup"><span data-stu-id="89ba7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89ba7-111">无</span><span class="sxs-lookup"><span data-stu-id="89ba7-111">none</span></span>|<span data-ttu-id="89ba7-112">0</span><span class="sxs-lookup"><span data-stu-id="89ba7-112">0</span></span>|<span data-ttu-id="89ba7-113">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="89ba7-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="89ba7-114">unknown</span><span class="sxs-lookup"><span data-stu-id="89ba7-114">unknown</span></span>|<span data-ttu-id="89ba7-115">1</span><span class="sxs-lookup"><span data-stu-id="89ba7-115">1</span></span>|<span data-ttu-id="89ba7-116">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="89ba7-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="89ba7-117">支持</span><span class="sxs-lookup"><span data-stu-id="89ba7-117">allowed</span></span>|<span data-ttu-id="89ba7-118">双面</span><span class="sxs-lookup"><span data-stu-id="89ba7-118">2</span></span>|<span data-ttu-id="89ba7-119">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="89ba7-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="89ba7-120">堵塞</span><span class="sxs-lookup"><span data-stu-id="89ba7-120">blocked</span></span>|<span data-ttu-id="89ba7-121">第三章</span><span class="sxs-lookup"><span data-stu-id="89ba7-121">3</span></span>|<span data-ttu-id="89ba7-122">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="89ba7-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="89ba7-123">隔离</span><span class="sxs-lookup"><span data-stu-id="89ba7-123">quarantined</span></span>|<span data-ttu-id="89ba7-124">4</span><span class="sxs-lookup"><span data-stu-id="89ba7-124">4</span></span>|<span data-ttu-id="89ba7-125">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="89ba7-125">Device is Quarantined in Exchange</span></span>|





