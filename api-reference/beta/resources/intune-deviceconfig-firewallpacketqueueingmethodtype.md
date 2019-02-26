---
title: firewallPacketQueueingMethodType 枚举类型
description: firewallPacketQueueingMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1b8543df5fa2a50cfdfa56c7cb2d96199ba44e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172203"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="982a0-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="982a0-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="982a0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="982a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="982a0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="982a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="982a0-106">firewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="982a0-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="982a0-107">成员</span><span class="sxs-lookup"><span data-stu-id="982a0-107">Members</span></span>
|<span data-ttu-id="982a0-108">成员</span><span class="sxs-lookup"><span data-stu-id="982a0-108">Member</span></span>|<span data-ttu-id="982a0-109">值</span><span class="sxs-lookup"><span data-stu-id="982a0-109">Value</span></span>|<span data-ttu-id="982a0-110">说明</span><span class="sxs-lookup"><span data-stu-id="982a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="982a0-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="982a0-111">deviceDefault</span></span>|<span data-ttu-id="982a0-112">0</span><span class="sxs-lookup"><span data-stu-id="982a0-112">0</span></span>|<span data-ttu-id="982a0-113">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="982a0-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="982a0-114">禁用</span><span class="sxs-lookup"><span data-stu-id="982a0-114">disabled</span></span>|<span data-ttu-id="982a0-115">1</span><span class="sxs-lookup"><span data-stu-id="982a0-115">1</span></span>|<span data-ttu-id="982a0-116">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="982a0-116">Disable packet queuing</span></span>|
|<span data-ttu-id="982a0-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="982a0-117">queueInbound</span></span>|<span data-ttu-id="982a0-118">双面</span><span class="sxs-lookup"><span data-stu-id="982a0-118">2</span></span>|<span data-ttu-id="982a0-119">对入站加密的数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="982a0-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="982a0-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="982a0-120">queueOutbound</span></span>|<span data-ttu-id="982a0-121">第三章</span><span class="sxs-lookup"><span data-stu-id="982a0-121">3</span></span>|<span data-ttu-id="982a0-122">队列解密出站数据包以供转发</span><span class="sxs-lookup"><span data-stu-id="982a0-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="982a0-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="982a0-123">queueBoth</span></span>|<span data-ttu-id="982a0-124">4</span><span class="sxs-lookup"><span data-stu-id="982a0-124">4</span></span>|<span data-ttu-id="982a0-125">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="982a0-125">Queue both inbound and outbound packets</span></span>|




