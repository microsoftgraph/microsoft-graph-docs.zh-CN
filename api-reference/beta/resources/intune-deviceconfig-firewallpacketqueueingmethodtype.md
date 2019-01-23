---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc40b93eebc17b1d1abcd9c317da1ffa538512a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425755"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="12346-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="12346-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="12346-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="12346-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="12346-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12346-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12346-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12346-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12346-107">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="12346-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="12346-108">成员</span><span class="sxs-lookup"><span data-stu-id="12346-108">Members</span></span>
|<span data-ttu-id="12346-109">成员</span><span class="sxs-lookup"><span data-stu-id="12346-109">Member</span></span>|<span data-ttu-id="12346-110">值</span><span class="sxs-lookup"><span data-stu-id="12346-110">Value</span></span>|<span data-ttu-id="12346-111">说明</span><span class="sxs-lookup"><span data-stu-id="12346-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12346-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="12346-112">deviceDefault</span></span>|<span data-ttu-id="12346-113">0</span><span class="sxs-lookup"><span data-stu-id="12346-113">0</span></span>|<span data-ttu-id="12346-114">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="12346-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="12346-115">禁用</span><span class="sxs-lookup"><span data-stu-id="12346-115">disabled</span></span>|<span data-ttu-id="12346-116">1</span><span class="sxs-lookup"><span data-stu-id="12346-116">1</span></span>|<span data-ttu-id="12346-117">停用数据包的队列</span><span class="sxs-lookup"><span data-stu-id="12346-117">Disable packet queuing</span></span>|
|<span data-ttu-id="12346-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="12346-118">queueInbound</span></span>|<span data-ttu-id="12346-119">2</span><span class="sxs-lookup"><span data-stu-id="12346-119">2</span></span>|<span data-ttu-id="12346-120">队列加密的入站的数据包</span><span class="sxs-lookup"><span data-stu-id="12346-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="12346-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="12346-121">queueOutbound</span></span>|<span data-ttu-id="12346-122">3</span><span class="sxs-lookup"><span data-stu-id="12346-122">3</span></span>|<span data-ttu-id="12346-123">用于呼叫转移队列解密出站数据包</span><span class="sxs-lookup"><span data-stu-id="12346-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="12346-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="12346-124">queueBoth</span></span>|<span data-ttu-id="12346-125">4</span><span class="sxs-lookup"><span data-stu-id="12346-125">4</span></span>|<span data-ttu-id="12346-126">队列入站和出站数据包</span><span class="sxs-lookup"><span data-stu-id="12346-126">Queue both inbound and outbound packets</span></span>|




