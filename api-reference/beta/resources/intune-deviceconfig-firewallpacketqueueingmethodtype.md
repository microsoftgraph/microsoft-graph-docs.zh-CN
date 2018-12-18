---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: tfitzmac
ms.openlocfilehash: 76d8e886c27e7e0e849a4172dbc763013f4cc5ac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347283"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="44e29-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="44e29-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="44e29-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="44e29-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44e29-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="44e29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44e29-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="44e29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44e29-107">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="44e29-107">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="44e29-108">成员</span><span class="sxs-lookup"><span data-stu-id="44e29-108">Members</span></span>
|<span data-ttu-id="44e29-109">成员</span><span class="sxs-lookup"><span data-stu-id="44e29-109">Member</span></span>|<span data-ttu-id="44e29-110">值</span><span class="sxs-lookup"><span data-stu-id="44e29-110">Value</span></span>|<span data-ttu-id="44e29-111">说明</span><span class="sxs-lookup"><span data-stu-id="44e29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44e29-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="44e29-112">deviceDefault</span></span>|<span data-ttu-id="44e29-113">0</span><span class="sxs-lookup"><span data-stu-id="44e29-113">0</span></span>|<span data-ttu-id="44e29-114">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="44e29-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="44e29-115">禁用</span><span class="sxs-lookup"><span data-stu-id="44e29-115">disabled</span></span>|<span data-ttu-id="44e29-116">1</span><span class="sxs-lookup"><span data-stu-id="44e29-116">1</span></span>|<span data-ttu-id="44e29-117">停用数据包的队列</span><span class="sxs-lookup"><span data-stu-id="44e29-117">Disable packet queuing</span></span>|
|<span data-ttu-id="44e29-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="44e29-118">queueInbound</span></span>|<span data-ttu-id="44e29-119">2</span><span class="sxs-lookup"><span data-stu-id="44e29-119">2</span></span>|<span data-ttu-id="44e29-120">队列加密的入站的数据包</span><span class="sxs-lookup"><span data-stu-id="44e29-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="44e29-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="44e29-121">queueOutbound</span></span>|<span data-ttu-id="44e29-122">3</span><span class="sxs-lookup"><span data-stu-id="44e29-122">3</span></span>|<span data-ttu-id="44e29-123">用于呼叫转移队列解密出站数据包</span><span class="sxs-lookup"><span data-stu-id="44e29-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="44e29-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="44e29-124">queueBoth</span></span>|<span data-ttu-id="44e29-125">4</span><span class="sxs-lookup"><span data-stu-id="44e29-125">4</span></span>|<span data-ttu-id="44e29-126">队列入站和出站数据包</span><span class="sxs-lookup"><span data-stu-id="44e29-126">Queue both inbound and outbound packets</span></span>|





