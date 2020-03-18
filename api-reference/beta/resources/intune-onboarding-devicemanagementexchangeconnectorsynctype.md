---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 57b3a31e7b80c546d17caf39c7269787367039e0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779119"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="14267-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="14267-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="14267-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14267-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14267-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14267-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14267-106">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="14267-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="14267-107">成员</span><span class="sxs-lookup"><span data-stu-id="14267-107">Members</span></span>
|<span data-ttu-id="14267-108">成员</span><span class="sxs-lookup"><span data-stu-id="14267-108">Member</span></span>|<span data-ttu-id="14267-109">值</span><span class="sxs-lookup"><span data-stu-id="14267-109">Value</span></span>|<span data-ttu-id="14267-110">说明</span><span class="sxs-lookup"><span data-stu-id="14267-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14267-111">完全同步</span><span class="sxs-lookup"><span data-stu-id="14267-111">fullSync</span></span>|<span data-ttu-id="14267-112">0</span><span class="sxs-lookup"><span data-stu-id="14267-112">0</span></span>|<span data-ttu-id="14267-113">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="14267-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="14267-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="14267-114">deltaSync</span></span>|<span data-ttu-id="14267-115">1</span><span class="sxs-lookup"><span data-stu-id="14267-115">1</span></span>|<span data-ttu-id="14267-116">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="14267-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



