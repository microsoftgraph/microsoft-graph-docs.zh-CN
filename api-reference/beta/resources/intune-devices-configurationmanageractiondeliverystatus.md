---
title: configurationManagerActionDeliveryStatus 枚举类型
description: Configuration Manager 设备操作的传递状态
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ab437ff9a7945b4bdd61b4e3e3a103e72b780e04
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465119"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a><span data-ttu-id="d1050-103">configurationManagerActionDeliveryStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d1050-103">configurationManagerActionDeliveryStatus enum type</span></span>

<span data-ttu-id="d1050-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1050-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1050-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1050-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1050-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1050-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1050-107">Configuration Manager 设备操作的传递状态</span><span class="sxs-lookup"><span data-stu-id="d1050-107">Delivery state of Configuration Manager device action</span></span>

## <a name="members"></a><span data-ttu-id="d1050-108">成员</span><span class="sxs-lookup"><span data-stu-id="d1050-108">Members</span></span>
|<span data-ttu-id="d1050-109">成员</span><span class="sxs-lookup"><span data-stu-id="d1050-109">Member</span></span>|<span data-ttu-id="d1050-110">值</span><span class="sxs-lookup"><span data-stu-id="d1050-110">Value</span></span>|<span data-ttu-id="d1050-111">说明</span><span class="sxs-lookup"><span data-stu-id="d1050-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1050-112">unknown</span><span class="sxs-lookup"><span data-stu-id="d1050-112">unknown</span></span>|<span data-ttu-id="d1050-113">0</span><span class="sxs-lookup"><span data-stu-id="d1050-113">0</span></span>|<span data-ttu-id="d1050-114">挂起，将操作传递给 ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="d1050-114">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="d1050-115">pendingDelivery</span><span class="sxs-lookup"><span data-stu-id="d1050-115">pendingDelivery</span></span>|<span data-ttu-id="d1050-116">1</span><span class="sxs-lookup"><span data-stu-id="d1050-116">1</span></span>|<span data-ttu-id="d1050-117">挂起，将操作传递给 ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="d1050-117">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="d1050-118">deliveredToConnectorService</span><span class="sxs-lookup"><span data-stu-id="d1050-118">deliveredToConnectorService</span></span>|<span data-ttu-id="d1050-119">双面</span><span class="sxs-lookup"><span data-stu-id="d1050-119">2</span></span>|<span data-ttu-id="d1050-120">将操作发送到 ConfigurationManager 连接器服务（云）</span><span class="sxs-lookup"><span data-stu-id="d1050-120">Action is sent to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="d1050-121">failedToDeliverToConnectorService</span><span class="sxs-lookup"><span data-stu-id="d1050-121">failedToDeliverToConnectorService</span></span>|<span data-ttu-id="d1050-122">第三章</span><span class="sxs-lookup"><span data-stu-id="d1050-122">3</span></span>|<span data-ttu-id="d1050-123">无法将操作发送到 ConfigurationManager 连接器服务（云）</span><span class="sxs-lookup"><span data-stu-id="d1050-123">Failed to send the action to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="d1050-124">deliveredToOnPremisesServer</span><span class="sxs-lookup"><span data-stu-id="d1050-124">deliveredToOnPremisesServer</span></span>|<span data-ttu-id="d1050-125">4 </span><span class="sxs-lookup"><span data-stu-id="d1050-125">4</span></span>|<span data-ttu-id="d1050-126">操作传递给 ConfigurationManager on-本地 server</span><span class="sxs-lookup"><span data-stu-id="d1050-126">Action is delivered to ConfigurationManager on-prem server</span></span>|



