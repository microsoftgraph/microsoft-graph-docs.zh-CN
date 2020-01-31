---
title: vpnServiceExceptionAction 枚举类型
description: 要对特定服务执行的 VPN 操作。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1310d91da9a7ea8e3a6274acd48e8ebc1359cafd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636712"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="53fcb-103">vpnServiceExceptionAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="53fcb-103">vpnServiceExceptionAction enum type</span></span>

> <span data-ttu-id="53fcb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="53fcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53fcb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53fcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53fcb-106">要对特定服务执行的 VPN 操作。</span><span class="sxs-lookup"><span data-stu-id="53fcb-106">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="53fcb-107">成员</span><span class="sxs-lookup"><span data-stu-id="53fcb-107">Members</span></span>
|<span data-ttu-id="53fcb-108">成员</span><span class="sxs-lookup"><span data-stu-id="53fcb-108">Member</span></span>|<span data-ttu-id="53fcb-109">值</span><span class="sxs-lookup"><span data-stu-id="53fcb-109">Value</span></span>|<span data-ttu-id="53fcb-110">Description</span><span class="sxs-lookup"><span data-stu-id="53fcb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53fcb-111">forceTrafficViaVPN</span><span class="sxs-lookup"><span data-stu-id="53fcb-111">forceTrafficViaVPN</span></span>|<span data-ttu-id="53fcb-112">0</span><span class="sxs-lookup"><span data-stu-id="53fcb-112">0</span></span>|<span data-ttu-id="53fcb-113">使来自该服务的所有流量都通过 VPN</span><span class="sxs-lookup"><span data-stu-id="53fcb-113">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="53fcb-114">allowTrafficOutside</span><span class="sxs-lookup"><span data-stu-id="53fcb-114">allowTrafficOutside</span></span>|<span data-ttu-id="53fcb-115">1 </span><span class="sxs-lookup"><span data-stu-id="53fcb-115">1</span></span>|<span data-ttu-id="53fcb-116">允许 VPN 外部的服务</span><span class="sxs-lookup"><span data-stu-id="53fcb-116">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="53fcb-117">dropTraffic</span><span class="sxs-lookup"><span data-stu-id="53fcb-117">dropTraffic</span></span>|<span data-ttu-id="53fcb-118">2 </span><span class="sxs-lookup"><span data-stu-id="53fcb-118">2</span></span>|<span data-ttu-id="53fcb-119">从服务中删除所有流量</span><span class="sxs-lookup"><span data-stu-id="53fcb-119">Drop all traffic from the service</span></span>|



