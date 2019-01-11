---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: Exchange 连接器同步请求的类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 33262ce8eb53b03af17a409d6fa5cd3e1dcd3357
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870579"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="68946-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="68946-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="68946-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="68946-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68946-105">Exchange 连接器同步请求的类型。</span><span class="sxs-lookup"><span data-stu-id="68946-105">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="68946-106">成员</span><span class="sxs-lookup"><span data-stu-id="68946-106">Members</span></span>
|<span data-ttu-id="68946-107">成员</span><span class="sxs-lookup"><span data-stu-id="68946-107">Member</span></span>|<span data-ttu-id="68946-108">值</span><span class="sxs-lookup"><span data-stu-id="68946-108">Value</span></span>|<span data-ttu-id="68946-109">Description</span><span class="sxs-lookup"><span data-stu-id="68946-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68946-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="68946-110">fullSync</span></span>|<span data-ttu-id="68946-111">0</span><span class="sxs-lookup"><span data-stu-id="68946-111">0</span></span>|<span data-ttu-id="68946-112">在 Exchange 中发现的所有设备。</span><span class="sxs-lookup"><span data-stu-id="68946-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="68946-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="68946-113">deltaSync</span></span>|<span data-ttu-id="68946-114">1</span><span class="sxs-lookup"><span data-stu-id="68946-114">1</span></span>|<span data-ttu-id="68946-115">发现其增量同步窗口期间已更新的 Exchange 中的设备。</span><span class="sxs-lookup"><span data-stu-id="68946-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



