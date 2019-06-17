---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4c7556fb3c37f9bfd564e31744f0e27a4482d6e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985848"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="f7202-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f7202-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="f7202-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7202-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7202-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7202-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7202-106">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="f7202-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="f7202-107">成员</span><span class="sxs-lookup"><span data-stu-id="f7202-107">Members</span></span>
|<span data-ttu-id="f7202-108">成员</span><span class="sxs-lookup"><span data-stu-id="f7202-108">Member</span></span>|<span data-ttu-id="f7202-109">值</span><span class="sxs-lookup"><span data-stu-id="f7202-109">Value</span></span>|<span data-ttu-id="f7202-110">说明</span><span class="sxs-lookup"><span data-stu-id="f7202-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7202-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f7202-111">deviceDefault</span></span>|<span data-ttu-id="f7202-112">0</span><span class="sxs-lookup"><span data-stu-id="f7202-112">0</span></span>|<span data-ttu-id="f7202-113">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="f7202-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="f7202-114">禁用</span><span class="sxs-lookup"><span data-stu-id="f7202-114">disabled</span></span>|<span data-ttu-id="f7202-115">1</span><span class="sxs-lookup"><span data-stu-id="f7202-115">1</span></span>|<span data-ttu-id="f7202-116">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="f7202-116">Disable packet queuing</span></span>|
|<span data-ttu-id="f7202-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="f7202-117">queueInbound</span></span>|<span data-ttu-id="f7202-118">双面</span><span class="sxs-lookup"><span data-stu-id="f7202-118">2</span></span>|<span data-ttu-id="f7202-119">对入站加密的数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="f7202-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="f7202-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="f7202-120">queueOutbound</span></span>|<span data-ttu-id="f7202-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f7202-121">3</span></span>|<span data-ttu-id="f7202-122">队列解密出站数据包以供转发</span><span class="sxs-lookup"><span data-stu-id="f7202-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="f7202-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="f7202-123">queueBoth</span></span>|<span data-ttu-id="f7202-124">4</span><span class="sxs-lookup"><span data-stu-id="f7202-124">4</span></span>|<span data-ttu-id="f7202-125">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="f7202-125">Queue both inbound and outbound packets</span></span>|





