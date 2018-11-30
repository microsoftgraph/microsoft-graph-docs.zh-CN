---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: Exchange 连接器同步请求的类型。
ms.openlocfilehash: 96117a7d11ca49cd39b60cb932bbb985ccf50d2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044429"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="04d04-103">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="04d04-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="04d04-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04d04-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04d04-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04d04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04d04-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="04d04-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04d04-107">Exchange 连接器同步请求的类型。</span><span class="sxs-lookup"><span data-stu-id="04d04-107">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="04d04-108">成员</span><span class="sxs-lookup"><span data-stu-id="04d04-108">Members</span></span>
|<span data-ttu-id="04d04-109">成员</span><span class="sxs-lookup"><span data-stu-id="04d04-109">Member</span></span>|<span data-ttu-id="04d04-110">值</span><span class="sxs-lookup"><span data-stu-id="04d04-110">Value</span></span>|<span data-ttu-id="04d04-111">说明</span><span class="sxs-lookup"><span data-stu-id="04d04-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04d04-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="04d04-112">fullSync</span></span>|<span data-ttu-id="04d04-113">0</span><span class="sxs-lookup"><span data-stu-id="04d04-113">0</span></span>|<span data-ttu-id="04d04-114">在 Exchange 中发现的所有设备。</span><span class="sxs-lookup"><span data-stu-id="04d04-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="04d04-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="04d04-115">deltaSync</span></span>|<span data-ttu-id="04d04-116">1</span><span class="sxs-lookup"><span data-stu-id="04d04-116">1</span></span>|<span data-ttu-id="04d04-117">发现其增量同步窗口期间已更新的 Exchange 中的设备。</span><span class="sxs-lookup"><span data-stu-id="04d04-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





