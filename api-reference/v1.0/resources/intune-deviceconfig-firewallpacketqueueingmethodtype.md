---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c3ed6ebdb4386c8203964ad1072767ec580dce2a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359227"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="69048-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="69048-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="69048-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69048-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69048-105">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="69048-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="69048-106">成员</span><span class="sxs-lookup"><span data-stu-id="69048-106">Members</span></span>
|<span data-ttu-id="69048-107">成员</span><span class="sxs-lookup"><span data-stu-id="69048-107">Member</span></span>|<span data-ttu-id="69048-108">值</span><span class="sxs-lookup"><span data-stu-id="69048-108">Value</span></span>|<span data-ttu-id="69048-109">说明</span><span class="sxs-lookup"><span data-stu-id="69048-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69048-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="69048-110">deviceDefault</span></span>|<span data-ttu-id="69048-111">0</span><span class="sxs-lookup"><span data-stu-id="69048-111">0</span></span>|<span data-ttu-id="69048-112">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="69048-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="69048-113">禁用</span><span class="sxs-lookup"><span data-stu-id="69048-113">disabled</span></span>|<span data-ttu-id="69048-114">1</span><span class="sxs-lookup"><span data-stu-id="69048-114">1</span></span>|<span data-ttu-id="69048-115">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="69048-115">Disable packet queuing</span></span>|
|<span data-ttu-id="69048-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="69048-116">queueInbound</span></span>|<span data-ttu-id="69048-117">双面</span><span class="sxs-lookup"><span data-stu-id="69048-117">2</span></span>|<span data-ttu-id="69048-118">对入站加密的数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="69048-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="69048-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="69048-119">queueOutbound</span></span>|<span data-ttu-id="69048-120">第三章</span><span class="sxs-lookup"><span data-stu-id="69048-120">3</span></span>|<span data-ttu-id="69048-121">队列解密出站数据包以供转发</span><span class="sxs-lookup"><span data-stu-id="69048-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="69048-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="69048-122">queueBoth</span></span>|<span data-ttu-id="69048-123">4</span><span class="sxs-lookup"><span data-stu-id="69048-123">4</span></span>|<span data-ttu-id="69048-124">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="69048-124">Queue both inbound and outbound packets</span></span>|




