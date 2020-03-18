---
title: configurationManagerActionDeliveryStatus 枚举类型
description: Configuration Manager 设备操作的传递状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58dca2b1ecb5419a3f56889a55c0816f492af430
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785089"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a><span data-ttu-id="46132-103">configurationManagerActionDeliveryStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="46132-103">configurationManagerActionDeliveryStatus enum type</span></span>

> <span data-ttu-id="46132-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="46132-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46132-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46132-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46132-106">Configuration Manager 设备操作的传递状态</span><span class="sxs-lookup"><span data-stu-id="46132-106">Delivery state of Configuration Manager device action</span></span>

## <a name="members"></a><span data-ttu-id="46132-107">成员</span><span class="sxs-lookup"><span data-stu-id="46132-107">Members</span></span>
|<span data-ttu-id="46132-108">成员</span><span class="sxs-lookup"><span data-stu-id="46132-108">Member</span></span>|<span data-ttu-id="46132-109">值</span><span class="sxs-lookup"><span data-stu-id="46132-109">Value</span></span>|<span data-ttu-id="46132-110">说明</span><span class="sxs-lookup"><span data-stu-id="46132-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46132-111">unknown</span><span class="sxs-lookup"><span data-stu-id="46132-111">unknown</span></span>|<span data-ttu-id="46132-112">0</span><span class="sxs-lookup"><span data-stu-id="46132-112">0</span></span>|<span data-ttu-id="46132-113">挂起，将操作传递给 ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="46132-113">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="46132-114">pendingDelivery</span><span class="sxs-lookup"><span data-stu-id="46132-114">pendingDelivery</span></span>|<span data-ttu-id="46132-115">1</span><span class="sxs-lookup"><span data-stu-id="46132-115">1</span></span>|<span data-ttu-id="46132-116">挂起，将操作传递给 ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="46132-116">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="46132-117">deliveredToConnectorService</span><span class="sxs-lookup"><span data-stu-id="46132-117">deliveredToConnectorService</span></span>|<span data-ttu-id="46132-118">双面</span><span class="sxs-lookup"><span data-stu-id="46132-118">2</span></span>|<span data-ttu-id="46132-119">将操作发送到 ConfigurationManager 连接器服务（云）</span><span class="sxs-lookup"><span data-stu-id="46132-119">Action is sent to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="46132-120">failedToDeliverToConnectorService</span><span class="sxs-lookup"><span data-stu-id="46132-120">failedToDeliverToConnectorService</span></span>|<span data-ttu-id="46132-121">第三章</span><span class="sxs-lookup"><span data-stu-id="46132-121">3</span></span>|<span data-ttu-id="46132-122">无法将操作发送到 ConfigurationManager 连接器服务（云）</span><span class="sxs-lookup"><span data-stu-id="46132-122">Failed to send the action to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="46132-123">deliveredToOnPremisesServer</span><span class="sxs-lookup"><span data-stu-id="46132-123">deliveredToOnPremisesServer</span></span>|<span data-ttu-id="46132-124">4 </span><span class="sxs-lookup"><span data-stu-id="46132-124">4</span></span>|<span data-ttu-id="46132-125">操作传递给 ConfigurationManager on-本地 server</span><span class="sxs-lookup"><span data-stu-id="46132-125">Action is delivered to ConfigurationManager on-prem server</span></span>|



