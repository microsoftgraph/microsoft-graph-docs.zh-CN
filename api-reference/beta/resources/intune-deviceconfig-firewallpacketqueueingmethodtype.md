---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b1802e150460e1e687b8303716a723146e4ca67
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946684"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="ca3de-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ca3de-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="ca3de-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca3de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca3de-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca3de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca3de-106">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="ca3de-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="ca3de-107">成员</span><span class="sxs-lookup"><span data-stu-id="ca3de-107">Members</span></span>
|<span data-ttu-id="ca3de-108">成员</span><span class="sxs-lookup"><span data-stu-id="ca3de-108">Member</span></span>|<span data-ttu-id="ca3de-109">值</span><span class="sxs-lookup"><span data-stu-id="ca3de-109">Value</span></span>|<span data-ttu-id="ca3de-110">说明</span><span class="sxs-lookup"><span data-stu-id="ca3de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca3de-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ca3de-111">deviceDefault</span></span>|<span data-ttu-id="ca3de-112">0</span><span class="sxs-lookup"><span data-stu-id="ca3de-112">0</span></span>|<span data-ttu-id="ca3de-113">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="ca3de-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="ca3de-114">禁用</span><span class="sxs-lookup"><span data-stu-id="ca3de-114">disabled</span></span>|<span data-ttu-id="ca3de-115">1</span><span class="sxs-lookup"><span data-stu-id="ca3de-115">1</span></span>|<span data-ttu-id="ca3de-116">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="ca3de-116">Disable packet queuing</span></span>|
|<span data-ttu-id="ca3de-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="ca3de-117">queueInbound</span></span>|<span data-ttu-id="ca3de-118">双面</span><span class="sxs-lookup"><span data-stu-id="ca3de-118">2</span></span>|<span data-ttu-id="ca3de-119">对入站加密的数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="ca3de-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="ca3de-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="ca3de-120">queueOutbound</span></span>|<span data-ttu-id="ca3de-121">第三章</span><span class="sxs-lookup"><span data-stu-id="ca3de-121">3</span></span>|<span data-ttu-id="ca3de-122">队列解密出站数据包以供转发</span><span class="sxs-lookup"><span data-stu-id="ca3de-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="ca3de-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="ca3de-123">queueBoth</span></span>|<span data-ttu-id="ca3de-124">4</span><span class="sxs-lookup"><span data-stu-id="ca3de-124">4</span></span>|<span data-ttu-id="ca3de-125">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="ca3de-125">Queue both inbound and outbound packets</span></span>|




