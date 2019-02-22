---
title: deviceManagementExchangeAccessLevel 枚举类型
description: Exchange 中的访问级别。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc84149f9ca6b178807e4bd70984fe1abfff6a09
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174233"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="d4bc1-103">deviceManagementExchangeAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d4bc1-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="d4bc1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d4bc1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4bc1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4bc1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4bc1-106">Exchange 中的访问级别。</span><span class="sxs-lookup"><span data-stu-id="d4bc1-106">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="d4bc1-107">成员</span><span class="sxs-lookup"><span data-stu-id="d4bc1-107">Members</span></span>
|<span data-ttu-id="d4bc1-108">成员</span><span class="sxs-lookup"><span data-stu-id="d4bc1-108">Member</span></span>|<span data-ttu-id="d4bc1-109">值</span><span class="sxs-lookup"><span data-stu-id="d4bc1-109">Value</span></span>|<span data-ttu-id="d4bc1-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4bc1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4bc1-111">无</span><span class="sxs-lookup"><span data-stu-id="d4bc1-111">none</span></span>|<span data-ttu-id="d4bc1-112">0</span><span class="sxs-lookup"><span data-stu-id="d4bc1-112">0</span></span>|<span data-ttu-id="d4bc1-113">未在 Exchange 中配置任何设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="d4bc1-113">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="d4bc1-114">允许</span><span class="sxs-lookup"><span data-stu-id="d4bc1-114">allow</span></span>|<span data-ttu-id="d4bc1-115">1</span><span class="sxs-lookup"><span data-stu-id="d4bc1-115">1</span></span>|<span data-ttu-id="d4bc1-116">允许设备访问 Exchange。</span><span class="sxs-lookup"><span data-stu-id="d4bc1-116">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="d4bc1-117">数据</span><span class="sxs-lookup"><span data-stu-id="d4bc1-117">block</span></span>|<span data-ttu-id="d4bc1-118">双面</span><span class="sxs-lookup"><span data-stu-id="d4bc1-118">2</span></span>|<span data-ttu-id="d4bc1-119">阻止设备访问 Exchange。</span><span class="sxs-lookup"><span data-stu-id="d4bc1-119">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="d4bc1-120">隔离</span><span class="sxs-lookup"><span data-stu-id="d4bc1-120">quarantine</span></span>|<span data-ttu-id="d4bc1-121">第三章</span><span class="sxs-lookup"><span data-stu-id="d4bc1-121">3</span></span>|<span data-ttu-id="d4bc1-122">隔离 Exchange 中的设备。</span><span class="sxs-lookup"><span data-stu-id="d4bc1-122">Quarantine the device in Exchange.</span></span>|




