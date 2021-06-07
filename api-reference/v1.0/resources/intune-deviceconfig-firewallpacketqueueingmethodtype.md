---
title: firewallPacketQueueingMethodType 枚举类型
description: firewallPacketQueueingMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a56e30f8b470271ea5fbb91765f7ea6814cbba14
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758853"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="11e2b-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="11e2b-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="11e2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11e2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11e2b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11e2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11e2b-106">firewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="11e2b-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="11e2b-107">成员</span><span class="sxs-lookup"><span data-stu-id="11e2b-107">Members</span></span>
|<span data-ttu-id="11e2b-108">成员</span><span class="sxs-lookup"><span data-stu-id="11e2b-108">Member</span></span>|<span data-ttu-id="11e2b-109">值</span><span class="sxs-lookup"><span data-stu-id="11e2b-109">Value</span></span>|<span data-ttu-id="11e2b-110">说明</span><span class="sxs-lookup"><span data-stu-id="11e2b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11e2b-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="11e2b-111">deviceDefault</span></span>|<span data-ttu-id="11e2b-112">0</span><span class="sxs-lookup"><span data-stu-id="11e2b-112">0</span></span>|<span data-ttu-id="11e2b-113">Intune 未配置任何值，请勿替代用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="11e2b-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="11e2b-114">disabled</span><span class="sxs-lookup"><span data-stu-id="11e2b-114">disabled</span></span>|<span data-ttu-id="11e2b-115">1</span><span class="sxs-lookup"><span data-stu-id="11e2b-115">1</span></span>|<span data-ttu-id="11e2b-116">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="11e2b-116">Disable packet queuing</span></span>|
|<span data-ttu-id="11e2b-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="11e2b-117">queueInbound</span></span>|<span data-ttu-id="11e2b-118">2</span><span class="sxs-lookup"><span data-stu-id="11e2b-118">2</span></span>|<span data-ttu-id="11e2b-119">将入站加密数据包排入队列</span><span class="sxs-lookup"><span data-stu-id="11e2b-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="11e2b-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="11e2b-120">queueOutbound</span></span>|<span data-ttu-id="11e2b-121">3</span><span class="sxs-lookup"><span data-stu-id="11e2b-121">3</span></span>|<span data-ttu-id="11e2b-122">队列解密的出站数据包用于转发</span><span class="sxs-lookup"><span data-stu-id="11e2b-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="11e2b-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="11e2b-123">queueBoth</span></span>|<span data-ttu-id="11e2b-124">4 </span><span class="sxs-lookup"><span data-stu-id="11e2b-124">4</span></span>|<span data-ttu-id="11e2b-125">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="11e2b-125">Queue both inbound and outbound packets</span></span>|




