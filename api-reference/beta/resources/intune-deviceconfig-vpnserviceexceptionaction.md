---
title: vpnServiceExceptionAction 枚举类型
description: 要对特定服务执行的 VPN 操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 079342d93ea96add59885079b4c6448145dbbe37
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736224"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="1b20c-103">vpnServiceExceptionAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1b20c-103">vpnServiceExceptionAction enum type</span></span>

<span data-ttu-id="1b20c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b20c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b20c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b20c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b20c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b20c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b20c-107">要对特定服务执行的 VPN 操作。</span><span class="sxs-lookup"><span data-stu-id="1b20c-107">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="1b20c-108">成员</span><span class="sxs-lookup"><span data-stu-id="1b20c-108">Members</span></span>
|<span data-ttu-id="1b20c-109">成员</span><span class="sxs-lookup"><span data-stu-id="1b20c-109">Member</span></span>|<span data-ttu-id="1b20c-110">值</span><span class="sxs-lookup"><span data-stu-id="1b20c-110">Value</span></span>|<span data-ttu-id="1b20c-111">说明</span><span class="sxs-lookup"><span data-stu-id="1b20c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b20c-112">forceTrafficViaVPN</span><span class="sxs-lookup"><span data-stu-id="1b20c-112">forceTrafficViaVPN</span></span>|<span data-ttu-id="1b20c-113">0</span><span class="sxs-lookup"><span data-stu-id="1b20c-113">0</span></span>|<span data-ttu-id="1b20c-114">使来自该服务的所有流量都通过 VPN</span><span class="sxs-lookup"><span data-stu-id="1b20c-114">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="1b20c-115">allowTrafficOutside</span><span class="sxs-lookup"><span data-stu-id="1b20c-115">allowTrafficOutside</span></span>|<span data-ttu-id="1b20c-116">1</span><span class="sxs-lookup"><span data-stu-id="1b20c-116">1</span></span>|<span data-ttu-id="1b20c-117">允许 VPN 外部的服务</span><span class="sxs-lookup"><span data-stu-id="1b20c-117">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="1b20c-118">dropTraffic</span><span class="sxs-lookup"><span data-stu-id="1b20c-118">dropTraffic</span></span>|<span data-ttu-id="1b20c-119">双面</span><span class="sxs-lookup"><span data-stu-id="1b20c-119">2</span></span>|<span data-ttu-id="1b20c-120">从服务中删除所有流量</span><span class="sxs-lookup"><span data-stu-id="1b20c-120">Drop all traffic from the service</span></span>|





