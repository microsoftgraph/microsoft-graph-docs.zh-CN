---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f4cde0b7d1d0ae6c728140c8e6b045b5a497a841
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448066"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="02fbc-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="02fbc-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

<span data-ttu-id="02fbc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02fbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02fbc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="02fbc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02fbc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02fbc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02fbc-107">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="02fbc-107">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="02fbc-108">成员</span><span class="sxs-lookup"><span data-stu-id="02fbc-108">Members</span></span>
|<span data-ttu-id="02fbc-109">成员</span><span class="sxs-lookup"><span data-stu-id="02fbc-109">Member</span></span>|<span data-ttu-id="02fbc-110">值</span><span class="sxs-lookup"><span data-stu-id="02fbc-110">Value</span></span>|<span data-ttu-id="02fbc-111">说明</span><span class="sxs-lookup"><span data-stu-id="02fbc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02fbc-112">完全同步</span><span class="sxs-lookup"><span data-stu-id="02fbc-112">fullSync</span></span>|<span data-ttu-id="02fbc-113">0</span><span class="sxs-lookup"><span data-stu-id="02fbc-113">0</span></span>|<span data-ttu-id="02fbc-114">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="02fbc-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="02fbc-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="02fbc-115">deltaSync</span></span>|<span data-ttu-id="02fbc-116">1</span><span class="sxs-lookup"><span data-stu-id="02fbc-116">1</span></span>|<span data-ttu-id="02fbc-117">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="02fbc-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



