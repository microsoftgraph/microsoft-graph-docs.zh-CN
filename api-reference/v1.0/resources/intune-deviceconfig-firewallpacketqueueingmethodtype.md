---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
ms.openlocfilehash: 70643e300f1a6cc151edeae849e5ae7c5f977750
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009832"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="b4a37-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b4a37-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="b4a37-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b4a37-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4a37-105">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="b4a37-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="b4a37-106">成员</span><span class="sxs-lookup"><span data-stu-id="b4a37-106">Members</span></span>
|<span data-ttu-id="b4a37-107">成员</span><span class="sxs-lookup"><span data-stu-id="b4a37-107">Member</span></span>|<span data-ttu-id="b4a37-108">值</span><span class="sxs-lookup"><span data-stu-id="b4a37-108">Value</span></span>|<span data-ttu-id="b4a37-109">说明</span><span class="sxs-lookup"><span data-stu-id="b4a37-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4a37-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b4a37-110">deviceDefault</span></span>|<span data-ttu-id="b4a37-111">0</span><span class="sxs-lookup"><span data-stu-id="b4a37-111">0</span></span>|<span data-ttu-id="b4a37-112">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="b4a37-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b4a37-113">禁用</span><span class="sxs-lookup"><span data-stu-id="b4a37-113">disabled</span></span>|<span data-ttu-id="b4a37-114">1</span><span class="sxs-lookup"><span data-stu-id="b4a37-114">1</span></span>|<span data-ttu-id="b4a37-115">停用数据包的队列</span><span class="sxs-lookup"><span data-stu-id="b4a37-115">Disable packet queuing</span></span>|
|<span data-ttu-id="b4a37-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="b4a37-116">queueInbound</span></span>|<span data-ttu-id="b4a37-117">2</span><span class="sxs-lookup"><span data-stu-id="b4a37-117">2</span></span>|<span data-ttu-id="b4a37-118">队列加密的入站的数据包</span><span class="sxs-lookup"><span data-stu-id="b4a37-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="b4a37-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="b4a37-119">queueOutbound</span></span>|<span data-ttu-id="b4a37-120">3</span><span class="sxs-lookup"><span data-stu-id="b4a37-120">3</span></span>|<span data-ttu-id="b4a37-121">用于呼叫转移队列解密出站数据包</span><span class="sxs-lookup"><span data-stu-id="b4a37-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="b4a37-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="b4a37-122">queueBoth</span></span>|<span data-ttu-id="b4a37-123">4</span><span class="sxs-lookup"><span data-stu-id="b4a37-123">4</span></span>|<span data-ttu-id="b4a37-124">队列入站和出站数据包</span><span class="sxs-lookup"><span data-stu-id="b4a37-124">Queue both inbound and outbound packets</span></span>|



