---
title: deviceManagementExchangeAccessLevel 枚举类型
description: Exchange 中的访问级别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 69a28cb03656ddaaf208e9d0f293b8a35b2c36ad
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029664"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="6d1a3-103">deviceManagementExchangeAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6d1a3-103">deviceManagementExchangeAccessLevel enum type</span></span>

<span data-ttu-id="6d1a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d1a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d1a3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6d1a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d1a3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d1a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d1a3-107">Exchange 中的访问级别。</span><span class="sxs-lookup"><span data-stu-id="6d1a3-107">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="6d1a3-108">成员</span><span class="sxs-lookup"><span data-stu-id="6d1a3-108">Members</span></span>
|<span data-ttu-id="6d1a3-109">成员</span><span class="sxs-lookup"><span data-stu-id="6d1a3-109">Member</span></span>|<span data-ttu-id="6d1a3-110">值</span><span class="sxs-lookup"><span data-stu-id="6d1a3-110">Value</span></span>|<span data-ttu-id="6d1a3-111">说明</span><span class="sxs-lookup"><span data-stu-id="6d1a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d1a3-112">无</span><span class="sxs-lookup"><span data-stu-id="6d1a3-112">none</span></span>|<span data-ttu-id="6d1a3-113">0</span><span class="sxs-lookup"><span data-stu-id="6d1a3-113">0</span></span>|<span data-ttu-id="6d1a3-114">未在 Exchange 中配置任何设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="6d1a3-114">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="6d1a3-115">允许</span><span class="sxs-lookup"><span data-stu-id="6d1a3-115">allow</span></span>|<span data-ttu-id="6d1a3-116">1 </span><span class="sxs-lookup"><span data-stu-id="6d1a3-116">1</span></span>|<span data-ttu-id="6d1a3-117">允许设备访问 Exchange。</span><span class="sxs-lookup"><span data-stu-id="6d1a3-117">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="6d1a3-118">数据</span><span class="sxs-lookup"><span data-stu-id="6d1a3-118">block</span></span>|<span data-ttu-id="6d1a3-119">2 </span><span class="sxs-lookup"><span data-stu-id="6d1a3-119">2</span></span>|<span data-ttu-id="6d1a3-120">阻止设备访问 Exchange。</span><span class="sxs-lookup"><span data-stu-id="6d1a3-120">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="6d1a3-121">隔离</span><span class="sxs-lookup"><span data-stu-id="6d1a3-121">quarantine</span></span>|<span data-ttu-id="6d1a3-122">第三章</span><span class="sxs-lookup"><span data-stu-id="6d1a3-122">3</span></span>|<span data-ttu-id="6d1a3-123">隔离 Exchange 中的设备。</span><span class="sxs-lookup"><span data-stu-id="6d1a3-123">Quarantine the device in Exchange.</span></span>|






