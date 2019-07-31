---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 86cdc6277232985d4c3e247c5c14801a5d3aef54
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010761"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="cd000-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cd000-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="cd000-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd000-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd000-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd000-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd000-106">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="cd000-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="cd000-107">成员</span><span class="sxs-lookup"><span data-stu-id="cd000-107">Members</span></span>
|<span data-ttu-id="cd000-108">成员</span><span class="sxs-lookup"><span data-stu-id="cd000-108">Member</span></span>|<span data-ttu-id="cd000-109">值</span><span class="sxs-lookup"><span data-stu-id="cd000-109">Value</span></span>|<span data-ttu-id="cd000-110">说明</span><span class="sxs-lookup"><span data-stu-id="cd000-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd000-111">完全同步</span><span class="sxs-lookup"><span data-stu-id="cd000-111">fullSync</span></span>|<span data-ttu-id="cd000-112">0</span><span class="sxs-lookup"><span data-stu-id="cd000-112">0</span></span>|<span data-ttu-id="cd000-113">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="cd000-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="cd000-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="cd000-114">deltaSync</span></span>|<span data-ttu-id="cd000-115">1</span><span class="sxs-lookup"><span data-stu-id="cd000-115">1</span></span>|<span data-ttu-id="cd000-116">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="cd000-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





