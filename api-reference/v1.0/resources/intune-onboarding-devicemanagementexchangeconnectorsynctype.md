---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8468c4580c39a8680253a4bb083ac1015b241df2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448107"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="052a3-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="052a3-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

<span data-ttu-id="052a3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="052a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="052a3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="052a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="052a3-106">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="052a3-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="052a3-107">成员</span><span class="sxs-lookup"><span data-stu-id="052a3-107">Members</span></span>
|<span data-ttu-id="052a3-108">成员</span><span class="sxs-lookup"><span data-stu-id="052a3-108">Member</span></span>|<span data-ttu-id="052a3-109">值</span><span class="sxs-lookup"><span data-stu-id="052a3-109">Value</span></span>|<span data-ttu-id="052a3-110">说明</span><span class="sxs-lookup"><span data-stu-id="052a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="052a3-111">完全同步</span><span class="sxs-lookup"><span data-stu-id="052a3-111">fullSync</span></span>|<span data-ttu-id="052a3-112">0</span><span class="sxs-lookup"><span data-stu-id="052a3-112">0</span></span>|<span data-ttu-id="052a3-113">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="052a3-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="052a3-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="052a3-114">deltaSync</span></span>|<span data-ttu-id="052a3-115">1 </span><span class="sxs-lookup"><span data-stu-id="052a3-115">1</span></span>|<span data-ttu-id="052a3-116">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="052a3-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




