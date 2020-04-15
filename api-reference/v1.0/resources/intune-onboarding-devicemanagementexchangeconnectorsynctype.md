---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3826680e05cc84054a874ae9357dfb0d50e88b57
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459481"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="edee1-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="edee1-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

<span data-ttu-id="edee1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edee1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edee1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edee1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edee1-106">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="edee1-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="edee1-107">成员</span><span class="sxs-lookup"><span data-stu-id="edee1-107">Members</span></span>
|<span data-ttu-id="edee1-108">成员</span><span class="sxs-lookup"><span data-stu-id="edee1-108">Member</span></span>|<span data-ttu-id="edee1-109">值</span><span class="sxs-lookup"><span data-stu-id="edee1-109">Value</span></span>|<span data-ttu-id="edee1-110">说明</span><span class="sxs-lookup"><span data-stu-id="edee1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edee1-111">完全同步</span><span class="sxs-lookup"><span data-stu-id="edee1-111">fullSync</span></span>|<span data-ttu-id="edee1-112">0</span><span class="sxs-lookup"><span data-stu-id="edee1-112">0</span></span>|<span data-ttu-id="edee1-113">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="edee1-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="edee1-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="edee1-114">deltaSync</span></span>|<span data-ttu-id="edee1-115">1</span><span class="sxs-lookup"><span data-stu-id="edee1-115">1</span></span>|<span data-ttu-id="edee1-116">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="edee1-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|







