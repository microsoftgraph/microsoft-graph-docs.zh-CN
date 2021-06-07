---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange 连接器同步的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4212f2c6d3e93f01de61519b04d83c0a61e03379
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751585"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="a4dff-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a4dff-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

<span data-ttu-id="a4dff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4dff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4dff-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4dff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4dff-106">请求的 Exchange 连接器同步的类型。</span><span class="sxs-lookup"><span data-stu-id="a4dff-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="a4dff-107">成员</span><span class="sxs-lookup"><span data-stu-id="a4dff-107">Members</span></span>
|<span data-ttu-id="a4dff-108">成员</span><span class="sxs-lookup"><span data-stu-id="a4dff-108">Member</span></span>|<span data-ttu-id="a4dff-109">值</span><span class="sxs-lookup"><span data-stu-id="a4dff-109">Value</span></span>|<span data-ttu-id="a4dff-110">Description</span><span class="sxs-lookup"><span data-stu-id="a4dff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4dff-111">fullSync</span><span class="sxs-lookup"><span data-stu-id="a4dff-111">fullSync</span></span>|<span data-ttu-id="a4dff-112">0</span><span class="sxs-lookup"><span data-stu-id="a4dff-112">0</span></span>|<span data-ttu-id="a4dff-113">发现设备中Exchange。</span><span class="sxs-lookup"><span data-stu-id="a4dff-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="a4dff-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="a4dff-114">deltaSync</span></span>|<span data-ttu-id="a4dff-115">1</span><span class="sxs-lookup"><span data-stu-id="a4dff-115">1</span></span>|<span data-ttu-id="a4dff-116">仅发现增量Exchange更新的设备。</span><span class="sxs-lookup"><span data-stu-id="a4dff-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




