---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: Exchange 连接器同步请求的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2a78bf79990eb16ae6dbc62d4c324b905a79a7f2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405623"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="ab9d4-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ab9d4-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="ab9d4-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ab9d4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab9d4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ab9d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab9d4-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab9d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab9d4-107">Exchange 连接器同步请求的类型。</span><span class="sxs-lookup"><span data-stu-id="ab9d4-107">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="ab9d4-108">成员</span><span class="sxs-lookup"><span data-stu-id="ab9d4-108">Members</span></span>
|<span data-ttu-id="ab9d4-109">成员</span><span class="sxs-lookup"><span data-stu-id="ab9d4-109">Member</span></span>|<span data-ttu-id="ab9d4-110">值</span><span class="sxs-lookup"><span data-stu-id="ab9d4-110">Value</span></span>|<span data-ttu-id="ab9d4-111">说明</span><span class="sxs-lookup"><span data-stu-id="ab9d4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab9d4-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="ab9d4-112">fullSync</span></span>|<span data-ttu-id="ab9d4-113">0</span><span class="sxs-lookup"><span data-stu-id="ab9d4-113">0</span></span>|<span data-ttu-id="ab9d4-114">在 Exchange 中发现的所有设备。</span><span class="sxs-lookup"><span data-stu-id="ab9d4-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="ab9d4-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="ab9d4-115">deltaSync</span></span>|<span data-ttu-id="ab9d4-116">1</span><span class="sxs-lookup"><span data-stu-id="ab9d4-116">1</span></span>|<span data-ttu-id="ab9d4-117">发现其增量同步窗口期间已更新的 Exchange 中的设备。</span><span class="sxs-lookup"><span data-stu-id="ab9d4-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




