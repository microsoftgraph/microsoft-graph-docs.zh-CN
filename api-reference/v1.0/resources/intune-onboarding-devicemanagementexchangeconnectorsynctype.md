---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e0ae6303c61b5e9b5a34eb559ad05aa32eb2051
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367978"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="ad283-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ad283-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="ad283-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ad283-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad283-105">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="ad283-105">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="ad283-106">成员</span><span class="sxs-lookup"><span data-stu-id="ad283-106">Members</span></span>
|<span data-ttu-id="ad283-107">成员</span><span class="sxs-lookup"><span data-stu-id="ad283-107">Member</span></span>|<span data-ttu-id="ad283-108">值</span><span class="sxs-lookup"><span data-stu-id="ad283-108">Value</span></span>|<span data-ttu-id="ad283-109">说明</span><span class="sxs-lookup"><span data-stu-id="ad283-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad283-110">完全同步</span><span class="sxs-lookup"><span data-stu-id="ad283-110">fullSync</span></span>|<span data-ttu-id="ad283-111">0</span><span class="sxs-lookup"><span data-stu-id="ad283-111">0</span></span>|<span data-ttu-id="ad283-112">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="ad283-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="ad283-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="ad283-113">deltaSync</span></span>|<span data-ttu-id="ad283-114">1</span><span class="sxs-lookup"><span data-stu-id="ad283-114">1</span></span>|<span data-ttu-id="ad283-115">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="ad283-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




