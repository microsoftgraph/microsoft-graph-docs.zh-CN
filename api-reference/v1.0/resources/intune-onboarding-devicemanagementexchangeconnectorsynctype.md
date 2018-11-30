---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: Exchange 连接器同步请求的类型。
ms.openlocfilehash: 123a1071db74e931cd80d8d735c83af8a7ef86f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009687"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="a8e12-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a8e12-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="a8e12-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a8e12-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8e12-105">Exchange 连接器同步请求的类型。</span><span class="sxs-lookup"><span data-stu-id="a8e12-105">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="a8e12-106">成员</span><span class="sxs-lookup"><span data-stu-id="a8e12-106">Members</span></span>
|<span data-ttu-id="a8e12-107">成员</span><span class="sxs-lookup"><span data-stu-id="a8e12-107">Member</span></span>|<span data-ttu-id="a8e12-108">值</span><span class="sxs-lookup"><span data-stu-id="a8e12-108">Value</span></span>|<span data-ttu-id="a8e12-109">说明</span><span class="sxs-lookup"><span data-stu-id="a8e12-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e12-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="a8e12-110">fullSync</span></span>|<span data-ttu-id="a8e12-111">0</span><span class="sxs-lookup"><span data-stu-id="a8e12-111">0</span></span>|<span data-ttu-id="a8e12-112">在 Exchange 中发现的所有设备。</span><span class="sxs-lookup"><span data-stu-id="a8e12-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="a8e12-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="a8e12-113">deltaSync</span></span>|<span data-ttu-id="a8e12-114">1</span><span class="sxs-lookup"><span data-stu-id="a8e12-114">1</span></span>|<span data-ttu-id="a8e12-115">发现其增量同步窗口期间已更新的 Exchange 中的设备。</span><span class="sxs-lookup"><span data-stu-id="a8e12-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



