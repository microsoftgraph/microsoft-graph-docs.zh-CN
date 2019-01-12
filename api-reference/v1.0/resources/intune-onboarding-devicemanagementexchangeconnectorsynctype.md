---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: Exchange 连接器同步请求的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5af14006bd6f3cc8733faecc8e0219cc02e7fcd9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983280"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="bddab-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bddab-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="bddab-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bddab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bddab-105">Exchange 连接器同步请求的类型。</span><span class="sxs-lookup"><span data-stu-id="bddab-105">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="bddab-106">成员</span><span class="sxs-lookup"><span data-stu-id="bddab-106">Members</span></span>
|<span data-ttu-id="bddab-107">成员</span><span class="sxs-lookup"><span data-stu-id="bddab-107">Member</span></span>|<span data-ttu-id="bddab-108">值</span><span class="sxs-lookup"><span data-stu-id="bddab-108">Value</span></span>|<span data-ttu-id="bddab-109">说明</span><span class="sxs-lookup"><span data-stu-id="bddab-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bddab-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="bddab-110">fullSync</span></span>|<span data-ttu-id="bddab-111">0</span><span class="sxs-lookup"><span data-stu-id="bddab-111">0</span></span>|<span data-ttu-id="bddab-112">在 Exchange 中发现的所有设备。</span><span class="sxs-lookup"><span data-stu-id="bddab-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="bddab-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="bddab-113">deltaSync</span></span>|<span data-ttu-id="bddab-114">1</span><span class="sxs-lookup"><span data-stu-id="bddab-114">1</span></span>|<span data-ttu-id="bddab-115">发现其增量同步窗口期间已更新的 Exchange 中的设备。</span><span class="sxs-lookup"><span data-stu-id="bddab-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



