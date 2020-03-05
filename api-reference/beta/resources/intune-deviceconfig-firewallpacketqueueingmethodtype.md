---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b134e00e0237e407331f0ea0554c54dcf0d39ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529993"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="5299e-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5299e-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="5299e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5299e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5299e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5299e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5299e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5299e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5299e-107">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="5299e-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="5299e-108">成员</span><span class="sxs-lookup"><span data-stu-id="5299e-108">Members</span></span>
|<span data-ttu-id="5299e-109">成员</span><span class="sxs-lookup"><span data-stu-id="5299e-109">Member</span></span>|<span data-ttu-id="5299e-110">值</span><span class="sxs-lookup"><span data-stu-id="5299e-110">Value</span></span>|<span data-ttu-id="5299e-111">说明</span><span class="sxs-lookup"><span data-stu-id="5299e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5299e-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="5299e-112">deviceDefault</span></span>|<span data-ttu-id="5299e-113">0</span><span class="sxs-lookup"><span data-stu-id="5299e-113">0</span></span>|<span data-ttu-id="5299e-114">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="5299e-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="5299e-115">禁用</span><span class="sxs-lookup"><span data-stu-id="5299e-115">disabled</span></span>|<span data-ttu-id="5299e-116">1 </span><span class="sxs-lookup"><span data-stu-id="5299e-116">1</span></span>|<span data-ttu-id="5299e-117">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="5299e-117">Disable packet queuing</span></span>|
|<span data-ttu-id="5299e-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="5299e-118">queueInbound</span></span>|<span data-ttu-id="5299e-119">2 </span><span class="sxs-lookup"><span data-stu-id="5299e-119">2</span></span>|<span data-ttu-id="5299e-120">对入站加密的数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="5299e-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="5299e-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="5299e-121">queueOutbound</span></span>|<span data-ttu-id="5299e-122">3 </span><span class="sxs-lookup"><span data-stu-id="5299e-122">3</span></span>|<span data-ttu-id="5299e-123">队列解密出站数据包以供转发</span><span class="sxs-lookup"><span data-stu-id="5299e-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="5299e-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="5299e-124">queueBoth</span></span>|<span data-ttu-id="5299e-125">4 </span><span class="sxs-lookup"><span data-stu-id="5299e-125">4</span></span>|<span data-ttu-id="5299e-126">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="5299e-126">Queue both inbound and outbound packets</span></span>|



