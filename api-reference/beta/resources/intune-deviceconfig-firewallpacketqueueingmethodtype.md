---
title: firewallPacketQueueingMethodType 枚举类型
description: firewallPacketQueueingMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2b83aa5d13ac170df1f9f99f8e430d10cdaba3e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460581"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="8f118-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8f118-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="8f118-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8f118-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f118-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f118-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f118-106">firewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="8f118-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="8f118-107">成员</span><span class="sxs-lookup"><span data-stu-id="8f118-107">Members</span></span>
|<span data-ttu-id="8f118-108">成员</span><span class="sxs-lookup"><span data-stu-id="8f118-108">Member</span></span>|<span data-ttu-id="8f118-109">值</span><span class="sxs-lookup"><span data-stu-id="8f118-109">Value</span></span>|<span data-ttu-id="8f118-110">说明</span><span class="sxs-lookup"><span data-stu-id="8f118-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f118-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="8f118-111">deviceDefault</span></span>|<span data-ttu-id="8f118-112">0</span><span class="sxs-lookup"><span data-stu-id="8f118-112">0</span></span>|<span data-ttu-id="8f118-113">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="8f118-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="8f118-114">禁用</span><span class="sxs-lookup"><span data-stu-id="8f118-114">disabled</span></span>|<span data-ttu-id="8f118-115">1</span><span class="sxs-lookup"><span data-stu-id="8f118-115">1</span></span>|<span data-ttu-id="8f118-116">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="8f118-116">Disable packet queuing</span></span>|
|<span data-ttu-id="8f118-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="8f118-117">queueInbound</span></span>|<span data-ttu-id="8f118-118">2 </span><span class="sxs-lookup"><span data-stu-id="8f118-118">2</span></span>|<span data-ttu-id="8f118-119">对入站加密的数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="8f118-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="8f118-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="8f118-120">queueOutbound</span></span>|<span data-ttu-id="8f118-121">3 </span><span class="sxs-lookup"><span data-stu-id="8f118-121">3</span></span>|<span data-ttu-id="8f118-122">队列解密出站数据包以供转发</span><span class="sxs-lookup"><span data-stu-id="8f118-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="8f118-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="8f118-123">queueBoth</span></span>|<span data-ttu-id="8f118-124">4 </span><span class="sxs-lookup"><span data-stu-id="8f118-124">4</span></span>|<span data-ttu-id="8f118-125">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="8f118-125">Queue both inbound and outbound packets</span></span>|





