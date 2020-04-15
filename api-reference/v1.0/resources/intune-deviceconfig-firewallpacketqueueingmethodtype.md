---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 110fffc41caa4efc6b7fbd9e1efe05f663cf8f85
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447722"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="02761-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="02761-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="02761-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02761-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02761-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02761-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02761-106">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="02761-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="02761-107">成员</span><span class="sxs-lookup"><span data-stu-id="02761-107">Members</span></span>
|<span data-ttu-id="02761-108">成员</span><span class="sxs-lookup"><span data-stu-id="02761-108">Member</span></span>|<span data-ttu-id="02761-109">值</span><span class="sxs-lookup"><span data-stu-id="02761-109">Value</span></span>|<span data-ttu-id="02761-110">说明</span><span class="sxs-lookup"><span data-stu-id="02761-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02761-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="02761-111">deviceDefault</span></span>|<span data-ttu-id="02761-112">0</span><span class="sxs-lookup"><span data-stu-id="02761-112">0</span></span>|<span data-ttu-id="02761-113">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="02761-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="02761-114">禁用</span><span class="sxs-lookup"><span data-stu-id="02761-114">disabled</span></span>|<span data-ttu-id="02761-115">1</span><span class="sxs-lookup"><span data-stu-id="02761-115">1</span></span>|<span data-ttu-id="02761-116">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="02761-116">Disable packet queuing</span></span>|
|<span data-ttu-id="02761-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="02761-117">queueInbound</span></span>|<span data-ttu-id="02761-118">双面</span><span class="sxs-lookup"><span data-stu-id="02761-118">2</span></span>|<span data-ttu-id="02761-119">对入站加密的数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="02761-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="02761-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="02761-120">queueOutbound</span></span>|<span data-ttu-id="02761-121">第三章</span><span class="sxs-lookup"><span data-stu-id="02761-121">3</span></span>|<span data-ttu-id="02761-122">队列解密出站数据包以供转发</span><span class="sxs-lookup"><span data-stu-id="02761-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="02761-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="02761-123">queueBoth</span></span>|<span data-ttu-id="02761-124">4 </span><span class="sxs-lookup"><span data-stu-id="02761-124">4</span></span>|<span data-ttu-id="02761-125">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="02761-125">Queue both inbound and outbound packets</span></span>|







