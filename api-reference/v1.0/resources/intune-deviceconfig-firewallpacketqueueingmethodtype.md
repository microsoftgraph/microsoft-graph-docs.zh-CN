---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 49fdf3172879092a04c20d0d73724744a9ef0fb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031561"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="fabb7-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fabb7-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="fabb7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fabb7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fabb7-105">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="fabb7-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="fabb7-106">成员</span><span class="sxs-lookup"><span data-stu-id="fabb7-106">Members</span></span>
|<span data-ttu-id="fabb7-107">成员</span><span class="sxs-lookup"><span data-stu-id="fabb7-107">Member</span></span>|<span data-ttu-id="fabb7-108">值</span><span class="sxs-lookup"><span data-stu-id="fabb7-108">Value</span></span>|<span data-ttu-id="fabb7-109">说明</span><span class="sxs-lookup"><span data-stu-id="fabb7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fabb7-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="fabb7-110">deviceDefault</span></span>|<span data-ttu-id="fabb7-111">0</span><span class="sxs-lookup"><span data-stu-id="fabb7-111">0</span></span>|<span data-ttu-id="fabb7-112">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="fabb7-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="fabb7-113">禁用</span><span class="sxs-lookup"><span data-stu-id="fabb7-113">disabled</span></span>|<span data-ttu-id="fabb7-114">1</span><span class="sxs-lookup"><span data-stu-id="fabb7-114">1</span></span>|<span data-ttu-id="fabb7-115">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="fabb7-115">Disable packet queuing</span></span>|
|<span data-ttu-id="fabb7-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="fabb7-116">queueInbound</span></span>|<span data-ttu-id="fabb7-117">双面</span><span class="sxs-lookup"><span data-stu-id="fabb7-117">2</span></span>|<span data-ttu-id="fabb7-118">对入站加密的数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="fabb7-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="fabb7-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="fabb7-119">queueOutbound</span></span>|<span data-ttu-id="fabb7-120">第三章</span><span class="sxs-lookup"><span data-stu-id="fabb7-120">3</span></span>|<span data-ttu-id="fabb7-121">队列解密出站数据包以供转发</span><span class="sxs-lookup"><span data-stu-id="fabb7-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="fabb7-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="fabb7-122">queueBoth</span></span>|<span data-ttu-id="fabb7-123">4</span><span class="sxs-lookup"><span data-stu-id="fabb7-123">4</span></span>|<span data-ttu-id="fabb7-124">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="fabb7-124">Queue both inbound and outbound packets</span></span>|



