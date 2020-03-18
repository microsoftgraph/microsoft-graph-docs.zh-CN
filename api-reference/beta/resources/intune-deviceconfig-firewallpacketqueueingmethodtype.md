---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8d4bd680061f49b91d9106f455487c72e3e7dbd7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791749"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="914de-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="914de-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="914de-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="914de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="914de-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="914de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="914de-106">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="914de-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="914de-107">成员</span><span class="sxs-lookup"><span data-stu-id="914de-107">Members</span></span>
|<span data-ttu-id="914de-108">成员</span><span class="sxs-lookup"><span data-stu-id="914de-108">Member</span></span>|<span data-ttu-id="914de-109">值</span><span class="sxs-lookup"><span data-stu-id="914de-109">Value</span></span>|<span data-ttu-id="914de-110">说明</span><span class="sxs-lookup"><span data-stu-id="914de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="914de-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="914de-111">deviceDefault</span></span>|<span data-ttu-id="914de-112">0</span><span class="sxs-lookup"><span data-stu-id="914de-112">0</span></span>|<span data-ttu-id="914de-113">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="914de-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="914de-114">禁用</span><span class="sxs-lookup"><span data-stu-id="914de-114">disabled</span></span>|<span data-ttu-id="914de-115">1</span><span class="sxs-lookup"><span data-stu-id="914de-115">1</span></span>|<span data-ttu-id="914de-116">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="914de-116">Disable packet queuing</span></span>|
|<span data-ttu-id="914de-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="914de-117">queueInbound</span></span>|<span data-ttu-id="914de-118">双面</span><span class="sxs-lookup"><span data-stu-id="914de-118">2</span></span>|<span data-ttu-id="914de-119">对入站加密的数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="914de-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="914de-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="914de-120">queueOutbound</span></span>|<span data-ttu-id="914de-121">第三章</span><span class="sxs-lookup"><span data-stu-id="914de-121">3</span></span>|<span data-ttu-id="914de-122">队列解密出站数据包以供转发</span><span class="sxs-lookup"><span data-stu-id="914de-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="914de-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="914de-123">queueBoth</span></span>|<span data-ttu-id="914de-124">4 </span><span class="sxs-lookup"><span data-stu-id="914de-124">4</span></span>|<span data-ttu-id="914de-125">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="914de-125">Queue both inbound and outbound packets</span></span>|



