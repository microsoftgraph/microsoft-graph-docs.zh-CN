---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: abb2a74c27df76a75971a2e2205698002bc3d8ab
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798458"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="635f0-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="635f0-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="635f0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="635f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="635f0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="635f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="635f0-106">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="635f0-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="635f0-107">成员</span><span class="sxs-lookup"><span data-stu-id="635f0-107">Members</span></span>
|<span data-ttu-id="635f0-108">成员</span><span class="sxs-lookup"><span data-stu-id="635f0-108">Member</span></span>|<span data-ttu-id="635f0-109">值</span><span class="sxs-lookup"><span data-stu-id="635f0-109">Value</span></span>|<span data-ttu-id="635f0-110">说明</span><span class="sxs-lookup"><span data-stu-id="635f0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="635f0-111">完全同步</span><span class="sxs-lookup"><span data-stu-id="635f0-111">fullSync</span></span>|<span data-ttu-id="635f0-112">0</span><span class="sxs-lookup"><span data-stu-id="635f0-112">0</span></span>|<span data-ttu-id="635f0-113">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="635f0-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="635f0-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="635f0-114">deltaSync</span></span>|<span data-ttu-id="635f0-115">1</span><span class="sxs-lookup"><span data-stu-id="635f0-115">1</span></span>|<span data-ttu-id="635f0-116">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="635f0-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





