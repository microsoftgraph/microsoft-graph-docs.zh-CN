---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1303287e521cf0b542047e8acaf122bc08a770a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823217"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="9198a-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9198a-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="9198a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9198a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9198a-105">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="9198a-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="9198a-106">成员</span><span class="sxs-lookup"><span data-stu-id="9198a-106">Members</span></span>
|<span data-ttu-id="9198a-107">成员</span><span class="sxs-lookup"><span data-stu-id="9198a-107">Member</span></span>|<span data-ttu-id="9198a-108">值</span><span class="sxs-lookup"><span data-stu-id="9198a-108">Value</span></span>|<span data-ttu-id="9198a-109">Description</span><span class="sxs-lookup"><span data-stu-id="9198a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9198a-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9198a-110">deviceDefault</span></span>|<span data-ttu-id="9198a-111">0</span><span class="sxs-lookup"><span data-stu-id="9198a-111">0</span></span>|<span data-ttu-id="9198a-112">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="9198a-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="9198a-113">禁用</span><span class="sxs-lookup"><span data-stu-id="9198a-113">disabled</span></span>|<span data-ttu-id="9198a-114">1</span><span class="sxs-lookup"><span data-stu-id="9198a-114">1</span></span>|<span data-ttu-id="9198a-115">停用数据包的队列</span><span class="sxs-lookup"><span data-stu-id="9198a-115">Disable packet queuing</span></span>|
|<span data-ttu-id="9198a-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="9198a-116">queueInbound</span></span>|<span data-ttu-id="9198a-117">2</span><span class="sxs-lookup"><span data-stu-id="9198a-117">2</span></span>|<span data-ttu-id="9198a-118">队列加密的入站的数据包</span><span class="sxs-lookup"><span data-stu-id="9198a-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="9198a-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="9198a-119">queueOutbound</span></span>|<span data-ttu-id="9198a-120">3</span><span class="sxs-lookup"><span data-stu-id="9198a-120">3</span></span>|<span data-ttu-id="9198a-121">用于呼叫转移队列解密出站数据包</span><span class="sxs-lookup"><span data-stu-id="9198a-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="9198a-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="9198a-122">queueBoth</span></span>|<span data-ttu-id="9198a-123">4</span><span class="sxs-lookup"><span data-stu-id="9198a-123">4</span></span>|<span data-ttu-id="9198a-124">队列入站和出站数据包</span><span class="sxs-lookup"><span data-stu-id="9198a-124">Queue both inbound and outbound packets</span></span>|



