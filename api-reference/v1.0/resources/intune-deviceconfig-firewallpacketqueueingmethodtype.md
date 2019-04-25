---
title: firewallPacketQueueingMethodType 枚举类型
description: firewallPacketQueueingMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdd9dc0279abc332bbf7b686f7f429fbd8db8883
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541306"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="53656-103">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="53656-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="53656-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53656-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53656-105">firewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="53656-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="53656-106">成员</span><span class="sxs-lookup"><span data-stu-id="53656-106">Members</span></span>
|<span data-ttu-id="53656-107">成员</span><span class="sxs-lookup"><span data-stu-id="53656-107">Member</span></span>|<span data-ttu-id="53656-108">值</span><span class="sxs-lookup"><span data-stu-id="53656-108">Value</span></span>|<span data-ttu-id="53656-109">说明</span><span class="sxs-lookup"><span data-stu-id="53656-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53656-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="53656-110">deviceDefault</span></span>|<span data-ttu-id="53656-111">0</span><span class="sxs-lookup"><span data-stu-id="53656-111">0</span></span>|<span data-ttu-id="53656-112">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="53656-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="53656-113">禁用</span><span class="sxs-lookup"><span data-stu-id="53656-113">disabled</span></span>|<span data-ttu-id="53656-114">1</span><span class="sxs-lookup"><span data-stu-id="53656-114">1</span></span>|<span data-ttu-id="53656-115">禁用数据包队列</span><span class="sxs-lookup"><span data-stu-id="53656-115">Disable packet queuing</span></span>|
|<span data-ttu-id="53656-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="53656-116">queueInbound</span></span>|<span data-ttu-id="53656-117">2 </span><span class="sxs-lookup"><span data-stu-id="53656-117">2</span></span>|<span data-ttu-id="53656-118">对入站加密的数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="53656-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="53656-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="53656-119">queueOutbound</span></span>|<span data-ttu-id="53656-120">3 </span><span class="sxs-lookup"><span data-stu-id="53656-120">3</span></span>|<span data-ttu-id="53656-121">队列解密出站数据包以供转发</span><span class="sxs-lookup"><span data-stu-id="53656-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="53656-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="53656-122">queueBoth</span></span>|<span data-ttu-id="53656-123">4 </span><span class="sxs-lookup"><span data-stu-id="53656-123">4</span></span>|<span data-ttu-id="53656-124">对入站和出站数据包进行排队</span><span class="sxs-lookup"><span data-stu-id="53656-124">Queue both inbound and outbound packets</span></span>|



