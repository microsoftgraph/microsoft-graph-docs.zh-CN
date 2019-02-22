---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47021a0a071995261f218cd4080026ababa33e0f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166596"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="b7d10-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b7d10-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="b7d10-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b7d10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7d10-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7d10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7d10-106">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="b7d10-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="b7d10-107">成员</span><span class="sxs-lookup"><span data-stu-id="b7d10-107">Members</span></span>
|<span data-ttu-id="b7d10-108">成员</span><span class="sxs-lookup"><span data-stu-id="b7d10-108">Member</span></span>|<span data-ttu-id="b7d10-109">值</span><span class="sxs-lookup"><span data-stu-id="b7d10-109">Value</span></span>|<span data-ttu-id="b7d10-110">说明</span><span class="sxs-lookup"><span data-stu-id="b7d10-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7d10-111">完全同步</span><span class="sxs-lookup"><span data-stu-id="b7d10-111">fullSync</span></span>|<span data-ttu-id="b7d10-112">0</span><span class="sxs-lookup"><span data-stu-id="b7d10-112">0</span></span>|<span data-ttu-id="b7d10-113">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="b7d10-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="b7d10-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="b7d10-114">deltaSync</span></span>|<span data-ttu-id="b7d10-115">1</span><span class="sxs-lookup"><span data-stu-id="b7d10-115">1</span></span>|<span data-ttu-id="b7d10-116">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="b7d10-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




