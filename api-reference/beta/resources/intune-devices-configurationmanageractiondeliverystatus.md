---
title: configurationManagerActionDeliveryStatus 枚举类型
description: Configuration Manager 设备操作的传递状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bbe36a6f7e346467d35bf997817241d7f30ef6df
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214624"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a><span data-ttu-id="44b2d-103">configurationManagerActionDeliveryStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="44b2d-103">configurationManagerActionDeliveryStatus enum type</span></span>

<span data-ttu-id="44b2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44b2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44b2d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="44b2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44b2d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44b2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44b2d-107">Configuration Manager 设备操作的传递状态</span><span class="sxs-lookup"><span data-stu-id="44b2d-107">Delivery state of Configuration Manager device action</span></span>

## <a name="members"></a><span data-ttu-id="44b2d-108">成员</span><span class="sxs-lookup"><span data-stu-id="44b2d-108">Members</span></span>
|<span data-ttu-id="44b2d-109">成员</span><span class="sxs-lookup"><span data-stu-id="44b2d-109">Member</span></span>|<span data-ttu-id="44b2d-110">值</span><span class="sxs-lookup"><span data-stu-id="44b2d-110">Value</span></span>|<span data-ttu-id="44b2d-111">说明</span><span class="sxs-lookup"><span data-stu-id="44b2d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44b2d-112">unknown</span><span class="sxs-lookup"><span data-stu-id="44b2d-112">unknown</span></span>|<span data-ttu-id="44b2d-113">0</span><span class="sxs-lookup"><span data-stu-id="44b2d-113">0</span></span>|<span data-ttu-id="44b2d-114">挂起，将操作传递给 ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="44b2d-114">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="44b2d-115">pendingDelivery</span><span class="sxs-lookup"><span data-stu-id="44b2d-115">pendingDelivery</span></span>|<span data-ttu-id="44b2d-116">1</span><span class="sxs-lookup"><span data-stu-id="44b2d-116">1</span></span>|<span data-ttu-id="44b2d-117">挂起，将操作传递给 ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="44b2d-117">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="44b2d-118">deliveredToConnectorService</span><span class="sxs-lookup"><span data-stu-id="44b2d-118">deliveredToConnectorService</span></span>|<span data-ttu-id="44b2d-119">双面</span><span class="sxs-lookup"><span data-stu-id="44b2d-119">2</span></span>|<span data-ttu-id="44b2d-120">将操作发送到 ConfigurationManager Connector service (云) </span><span class="sxs-lookup"><span data-stu-id="44b2d-120">Action is sent to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="44b2d-121">failedToDeliverToConnectorService</span><span class="sxs-lookup"><span data-stu-id="44b2d-121">failedToDeliverToConnectorService</span></span>|<span data-ttu-id="44b2d-122">第三章</span><span class="sxs-lookup"><span data-stu-id="44b2d-122">3</span></span>|<span data-ttu-id="44b2d-123">无法将操作发送到 ConfigurationManager Connector service (云) </span><span class="sxs-lookup"><span data-stu-id="44b2d-123">Failed to send the action to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="44b2d-124">deliveredToOnPremisesServer</span><span class="sxs-lookup"><span data-stu-id="44b2d-124">deliveredToOnPremisesServer</span></span>|<span data-ttu-id="44b2d-125">4 </span><span class="sxs-lookup"><span data-stu-id="44b2d-125">4</span></span>|<span data-ttu-id="44b2d-126">操作传递给 ConfigurationManager on-本地 server</span><span class="sxs-lookup"><span data-stu-id="44b2d-126">Action is delivered to ConfigurationManager on-prem server</span></span>|




