---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfdd1da2ecec6fb7848787386991ee09741d0b67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565925"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="c6b3b-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c6b3b-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="c6b3b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6b3b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6b3b-105">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="c6b3b-105">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="c6b3b-106">成员</span><span class="sxs-lookup"><span data-stu-id="c6b3b-106">Members</span></span>
|<span data-ttu-id="c6b3b-107">成员</span><span class="sxs-lookup"><span data-stu-id="c6b3b-107">Member</span></span>|<span data-ttu-id="c6b3b-108">值</span><span class="sxs-lookup"><span data-stu-id="c6b3b-108">Value</span></span>|<span data-ttu-id="c6b3b-109">说明</span><span class="sxs-lookup"><span data-stu-id="c6b3b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6b3b-110">完全同步</span><span class="sxs-lookup"><span data-stu-id="c6b3b-110">fullSync</span></span>|<span data-ttu-id="c6b3b-111">0</span><span class="sxs-lookup"><span data-stu-id="c6b3b-111">0</span></span>|<span data-ttu-id="c6b3b-112">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="c6b3b-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="c6b3b-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="c6b3b-113">deltaSync</span></span>|<span data-ttu-id="c6b3b-114">1</span><span class="sxs-lookup"><span data-stu-id="c6b3b-114">1</span></span>|<span data-ttu-id="c6b3b-115">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="c6b3b-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



