---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: tfitzmac
ms.openlocfilehash: 9f3d63b7e58b6f9c5ba369c3ceb12d06704c4725
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304555"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="38703-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="38703-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="38703-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="38703-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38703-105">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="38703-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="38703-106">成员</span><span class="sxs-lookup"><span data-stu-id="38703-106">Members</span></span>
|<span data-ttu-id="38703-107">成员</span><span class="sxs-lookup"><span data-stu-id="38703-107">Member</span></span>|<span data-ttu-id="38703-108">值</span><span class="sxs-lookup"><span data-stu-id="38703-108">Value</span></span>|<span data-ttu-id="38703-109">说明</span><span class="sxs-lookup"><span data-stu-id="38703-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38703-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="38703-110">deviceDefault</span></span>|<span data-ttu-id="38703-111">0</span><span class="sxs-lookup"><span data-stu-id="38703-111">0</span></span>|<span data-ttu-id="38703-112">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="38703-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="38703-113">禁用</span><span class="sxs-lookup"><span data-stu-id="38703-113">disabled</span></span>|<span data-ttu-id="38703-114">1</span><span class="sxs-lookup"><span data-stu-id="38703-114">1</span></span>|<span data-ttu-id="38703-115">停用数据包的队列</span><span class="sxs-lookup"><span data-stu-id="38703-115">Disable packet queuing</span></span>|
|<span data-ttu-id="38703-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="38703-116">queueInbound</span></span>|<span data-ttu-id="38703-117">2</span><span class="sxs-lookup"><span data-stu-id="38703-117">2</span></span>|<span data-ttu-id="38703-118">队列加密的入站的数据包</span><span class="sxs-lookup"><span data-stu-id="38703-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="38703-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="38703-119">queueOutbound</span></span>|<span data-ttu-id="38703-120">3</span><span class="sxs-lookup"><span data-stu-id="38703-120">3</span></span>|<span data-ttu-id="38703-121">用于呼叫转移队列解密出站数据包</span><span class="sxs-lookup"><span data-stu-id="38703-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="38703-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="38703-122">queueBoth</span></span>|<span data-ttu-id="38703-123">4</span><span class="sxs-lookup"><span data-stu-id="38703-123">4</span></span>|<span data-ttu-id="38703-124">队列入站和出站数据包</span><span class="sxs-lookup"><span data-stu-id="38703-124">Queue both inbound and outbound packets</span></span>|



