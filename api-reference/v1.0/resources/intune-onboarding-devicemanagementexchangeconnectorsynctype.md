---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 939ff7fe3a65da9bd66b29c2258f135275ac855f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056539"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="edc3b-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="edc3b-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

<span data-ttu-id="edc3b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edc3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edc3b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edc3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edc3b-106">请求的 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="edc3b-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="edc3b-107">成员</span><span class="sxs-lookup"><span data-stu-id="edc3b-107">Members</span></span>
|<span data-ttu-id="edc3b-108">成员</span><span class="sxs-lookup"><span data-stu-id="edc3b-108">Member</span></span>|<span data-ttu-id="edc3b-109">值</span><span class="sxs-lookup"><span data-stu-id="edc3b-109">Value</span></span>|<span data-ttu-id="edc3b-110">说明</span><span class="sxs-lookup"><span data-stu-id="edc3b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edc3b-111">完全同步</span><span class="sxs-lookup"><span data-stu-id="edc3b-111">fullSync</span></span>|<span data-ttu-id="edc3b-112">0</span><span class="sxs-lookup"><span data-stu-id="edc3b-112">0</span></span>|<span data-ttu-id="edc3b-113">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="edc3b-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="edc3b-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="edc3b-114">deltaSync</span></span>|<span data-ttu-id="edc3b-115">1 </span><span class="sxs-lookup"><span data-stu-id="edc3b-115">1</span></span>|<span data-ttu-id="edc3b-116">仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。</span><span class="sxs-lookup"><span data-stu-id="edc3b-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|









