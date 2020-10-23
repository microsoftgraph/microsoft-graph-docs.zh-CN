---
title: configurationManagerActionDeliveryStatus 枚举类型
description: Configuration Manager 设备操作的传递状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 09c7b1be3a5fdfc33a064d2a9208daa68ba4263e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733984"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a><span data-ttu-id="e76d4-103">configurationManagerActionDeliveryStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e76d4-103">configurationManagerActionDeliveryStatus enum type</span></span>

<span data-ttu-id="e76d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e76d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e76d4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e76d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e76d4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e76d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e76d4-107">Configuration Manager 设备操作的传递状态</span><span class="sxs-lookup"><span data-stu-id="e76d4-107">Delivery state of Configuration Manager device action</span></span>

## <a name="members"></a><span data-ttu-id="e76d4-108">成员</span><span class="sxs-lookup"><span data-stu-id="e76d4-108">Members</span></span>
|<span data-ttu-id="e76d4-109">成员</span><span class="sxs-lookup"><span data-stu-id="e76d4-109">Member</span></span>|<span data-ttu-id="e76d4-110">值</span><span class="sxs-lookup"><span data-stu-id="e76d4-110">Value</span></span>|<span data-ttu-id="e76d4-111">说明</span><span class="sxs-lookup"><span data-stu-id="e76d4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e76d4-112">unknown</span><span class="sxs-lookup"><span data-stu-id="e76d4-112">unknown</span></span>|<span data-ttu-id="e76d4-113">0</span><span class="sxs-lookup"><span data-stu-id="e76d4-113">0</span></span>|<span data-ttu-id="e76d4-114">挂起，将操作传递给 ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="e76d4-114">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="e76d4-115">pendingDelivery</span><span class="sxs-lookup"><span data-stu-id="e76d4-115">pendingDelivery</span></span>|<span data-ttu-id="e76d4-116">1</span><span class="sxs-lookup"><span data-stu-id="e76d4-116">1</span></span>|<span data-ttu-id="e76d4-117">挂起，将操作传递给 ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="e76d4-117">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="e76d4-118">deliveredToConnectorService</span><span class="sxs-lookup"><span data-stu-id="e76d4-118">deliveredToConnectorService</span></span>|<span data-ttu-id="e76d4-119">双面</span><span class="sxs-lookup"><span data-stu-id="e76d4-119">2</span></span>|<span data-ttu-id="e76d4-120">将操作发送到 ConfigurationManager Connector service (云) </span><span class="sxs-lookup"><span data-stu-id="e76d4-120">Action is sent to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="e76d4-121">failedToDeliverToConnectorService</span><span class="sxs-lookup"><span data-stu-id="e76d4-121">failedToDeliverToConnectorService</span></span>|<span data-ttu-id="e76d4-122">第三章</span><span class="sxs-lookup"><span data-stu-id="e76d4-122">3</span></span>|<span data-ttu-id="e76d4-123">无法将操作发送到 ConfigurationManager Connector service (云) </span><span class="sxs-lookup"><span data-stu-id="e76d4-123">Failed to send the action to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="e76d4-124">deliveredToOnPremisesServer</span><span class="sxs-lookup"><span data-stu-id="e76d4-124">deliveredToOnPremisesServer</span></span>|<span data-ttu-id="e76d4-125">4 </span><span class="sxs-lookup"><span data-stu-id="e76d4-125">4</span></span>|<span data-ttu-id="e76d4-126">操作传递给 ConfigurationManager on-本地 server</span><span class="sxs-lookup"><span data-stu-id="e76d4-126">Action is delivered to ConfigurationManager on-prem server</span></span>|





