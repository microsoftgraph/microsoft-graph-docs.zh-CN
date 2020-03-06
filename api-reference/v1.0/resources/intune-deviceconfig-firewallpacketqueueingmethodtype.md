---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0b5976d7ff06620db9958dacdfdd0b8b0c81a191
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530727"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="79ffc-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="79ffc-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="79ffc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79ffc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79ffc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79ffc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79ffc-106">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="79ffc-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="79ffc-107">成员</span><span class="sxs-lookup"><span data-stu-id="79ffc-107">Members</span></span>
|<span data-ttu-id="79ffc-108">成员</span><span class="sxs-lookup"><span data-stu-id="79ffc-108">Member</span></span>|<span data-ttu-id="79ffc-109">值</span><span class="sxs-lookup"><span data-stu-id="79ffc-109">Value</span></span>|<span data-ttu-id="79ffc-110">说明</span><span class="sxs-lookup"><span data-stu-id="79ffc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79ffc-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="79ffc-111">deviceDefault</span></span>|<span data-ttu-id="79ffc-112">0</span><span class="sxs-lookup"><span data-stu-id="79ffc-112">0</span></span>|<span data-ttu-id="79ffc-113">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="79ffc-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="79ffc-114">禁用</span><span class="sxs-lookup"><span data-stu-id="79ffc-114">disabled</span></span>|<span data-ttu-id="79ffc-115">1 </span><span class="sxs-lookup"><span data-stu-id="79ffc-115">1</span></span>|<span data-ttu-id="79ffc-116">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="79ffc-116">Disable packet queuing</span></span>|
|<span data-ttu-id="79ffc-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="79ffc-117">queueInbound</span></span>|<span data-ttu-id="79ffc-118">2 </span><span class="sxs-lookup"><span data-stu-id="79ffc-118">2</span></span>|<span data-ttu-id="79ffc-119">对入站加密的数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="79ffc-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="79ffc-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="79ffc-120">queueOutbound</span></span>|<span data-ttu-id="79ffc-121">3 </span><span class="sxs-lookup"><span data-stu-id="79ffc-121">3</span></span>|<span data-ttu-id="79ffc-122">队列解密出站数据包以供转发</span><span class="sxs-lookup"><span data-stu-id="79ffc-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="79ffc-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="79ffc-123">queueBoth</span></span>|<span data-ttu-id="79ffc-124">4 </span><span class="sxs-lookup"><span data-stu-id="79ffc-124">4</span></span>|<span data-ttu-id="79ffc-125">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="79ffc-125">Queue both inbound and outbound packets</span></span>|




