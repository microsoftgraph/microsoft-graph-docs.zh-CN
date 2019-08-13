---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f68277b2eeb7aea123ee843a0b602d11123cbd04
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369449"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="1f312-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1f312-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="1f312-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1f312-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f312-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f312-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f312-106">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="1f312-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="1f312-107">成员</span><span class="sxs-lookup"><span data-stu-id="1f312-107">Members</span></span>
|<span data-ttu-id="1f312-108">成员</span><span class="sxs-lookup"><span data-stu-id="1f312-108">Member</span></span>|<span data-ttu-id="1f312-109">值</span><span class="sxs-lookup"><span data-stu-id="1f312-109">Value</span></span>|<span data-ttu-id="1f312-110">说明</span><span class="sxs-lookup"><span data-stu-id="1f312-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f312-111">完全同步</span><span class="sxs-lookup"><span data-stu-id="1f312-111">fullSync</span></span>|<span data-ttu-id="1f312-112">0</span><span class="sxs-lookup"><span data-stu-id="1f312-112">0</span></span>|<span data-ttu-id="1f312-113">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="1f312-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="1f312-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="1f312-114">deltaSync</span></span>|<span data-ttu-id="1f312-115">1</span><span class="sxs-lookup"><span data-stu-id="1f312-115">1</span></span>|<span data-ttu-id="1f312-116">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="1f312-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



