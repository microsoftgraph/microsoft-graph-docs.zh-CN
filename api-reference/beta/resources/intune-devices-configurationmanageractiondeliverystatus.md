---
title: configurationManagerActionDeliveryStatus 枚举类型
description: Configuration Manager 设备操作的传递状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1751f4e53c3df3b3a27d759ff9f747ead5360211
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060690"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a><span data-ttu-id="91fe2-103">configurationManagerActionDeliveryStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="91fe2-103">configurationManagerActionDeliveryStatus enum type</span></span>

<span data-ttu-id="91fe2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91fe2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91fe2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="91fe2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91fe2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91fe2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91fe2-107">Configuration Manager 设备操作的传递状态</span><span class="sxs-lookup"><span data-stu-id="91fe2-107">Delivery state of Configuration Manager device action</span></span>

## <a name="members"></a><span data-ttu-id="91fe2-108">成员</span><span class="sxs-lookup"><span data-stu-id="91fe2-108">Members</span></span>
|<span data-ttu-id="91fe2-109">成员</span><span class="sxs-lookup"><span data-stu-id="91fe2-109">Member</span></span>|<span data-ttu-id="91fe2-110">值</span><span class="sxs-lookup"><span data-stu-id="91fe2-110">Value</span></span>|<span data-ttu-id="91fe2-111">说明</span><span class="sxs-lookup"><span data-stu-id="91fe2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91fe2-112">unknown</span><span class="sxs-lookup"><span data-stu-id="91fe2-112">unknown</span></span>|<span data-ttu-id="91fe2-113">0</span><span class="sxs-lookup"><span data-stu-id="91fe2-113">0</span></span>|<span data-ttu-id="91fe2-114">挂起，将操作传递给 ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="91fe2-114">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="91fe2-115">pendingDelivery</span><span class="sxs-lookup"><span data-stu-id="91fe2-115">pendingDelivery</span></span>|<span data-ttu-id="91fe2-116">1 </span><span class="sxs-lookup"><span data-stu-id="91fe2-116">1</span></span>|<span data-ttu-id="91fe2-117">挂起，将操作传递给 ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="91fe2-117">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="91fe2-118">deliveredToConnectorService</span><span class="sxs-lookup"><span data-stu-id="91fe2-118">deliveredToConnectorService</span></span>|<span data-ttu-id="91fe2-119">2 </span><span class="sxs-lookup"><span data-stu-id="91fe2-119">2</span></span>|<span data-ttu-id="91fe2-120">将操作发送到 ConfigurationManager Connector service (云) </span><span class="sxs-lookup"><span data-stu-id="91fe2-120">Action is sent to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="91fe2-121">failedToDeliverToConnectorService</span><span class="sxs-lookup"><span data-stu-id="91fe2-121">failedToDeliverToConnectorService</span></span>|<span data-ttu-id="91fe2-122">第三章</span><span class="sxs-lookup"><span data-stu-id="91fe2-122">3</span></span>|<span data-ttu-id="91fe2-123">无法将操作发送到 ConfigurationManager Connector service (云) </span><span class="sxs-lookup"><span data-stu-id="91fe2-123">Failed to send the action to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="91fe2-124">deliveredToOnPremisesServer</span><span class="sxs-lookup"><span data-stu-id="91fe2-124">deliveredToOnPremisesServer</span></span>|<span data-ttu-id="91fe2-125">4 </span><span class="sxs-lookup"><span data-stu-id="91fe2-125">4</span></span>|<span data-ttu-id="91fe2-126">操作传递给 ConfigurationManager on-本地 server</span><span class="sxs-lookup"><span data-stu-id="91fe2-126">Action is delivered to ConfigurationManager on-prem server</span></span>|






