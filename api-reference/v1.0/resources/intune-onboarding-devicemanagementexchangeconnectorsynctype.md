---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: Exchange 连接器同步请求的类型。
author: tfitzmac
ms.openlocfilehash: 1915de3305cb8e41609dd2101f246a8e003f60f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312073"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="17b1b-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="17b1b-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="17b1b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="17b1b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17b1b-105">Exchange 连接器同步请求的类型。</span><span class="sxs-lookup"><span data-stu-id="17b1b-105">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="17b1b-106">成员</span><span class="sxs-lookup"><span data-stu-id="17b1b-106">Members</span></span>
|<span data-ttu-id="17b1b-107">成员</span><span class="sxs-lookup"><span data-stu-id="17b1b-107">Member</span></span>|<span data-ttu-id="17b1b-108">值</span><span class="sxs-lookup"><span data-stu-id="17b1b-108">Value</span></span>|<span data-ttu-id="17b1b-109">说明</span><span class="sxs-lookup"><span data-stu-id="17b1b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17b1b-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="17b1b-110">fullSync</span></span>|<span data-ttu-id="17b1b-111">0</span><span class="sxs-lookup"><span data-stu-id="17b1b-111">0</span></span>|<span data-ttu-id="17b1b-112">在 Exchange 中发现的所有设备。</span><span class="sxs-lookup"><span data-stu-id="17b1b-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="17b1b-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="17b1b-113">deltaSync</span></span>|<span data-ttu-id="17b1b-114">1</span><span class="sxs-lookup"><span data-stu-id="17b1b-114">1</span></span>|<span data-ttu-id="17b1b-115">发现其增量同步窗口期间已更新的 Exchange 中的设备。</span><span class="sxs-lookup"><span data-stu-id="17b1b-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



