---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 148a99b73064bf54812a851ea707090617bea584
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527747"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="447bf-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="447bf-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

<span data-ttu-id="447bf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="447bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="447bf-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="447bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="447bf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="447bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="447bf-107">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="447bf-107">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="447bf-108">成员</span><span class="sxs-lookup"><span data-stu-id="447bf-108">Members</span></span>
|<span data-ttu-id="447bf-109">成员</span><span class="sxs-lookup"><span data-stu-id="447bf-109">Member</span></span>|<span data-ttu-id="447bf-110">值</span><span class="sxs-lookup"><span data-stu-id="447bf-110">Value</span></span>|<span data-ttu-id="447bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="447bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="447bf-112">完全同步</span><span class="sxs-lookup"><span data-stu-id="447bf-112">fullSync</span></span>|<span data-ttu-id="447bf-113">0</span><span class="sxs-lookup"><span data-stu-id="447bf-113">0</span></span>|<span data-ttu-id="447bf-114">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="447bf-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="447bf-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="447bf-115">deltaSync</span></span>|<span data-ttu-id="447bf-116">1 </span><span class="sxs-lookup"><span data-stu-id="447bf-116">1</span></span>|<span data-ttu-id="447bf-117">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="447bf-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



