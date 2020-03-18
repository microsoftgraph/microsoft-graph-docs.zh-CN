---
title: vpnServiceExceptionAction 枚举类型
description: 要对特定服务执行的 VPN 操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b0c952a14db65e836c2a3391cb44a871957e708
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787304"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="b13dc-103">vpnServiceExceptionAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b13dc-103">vpnServiceExceptionAction enum type</span></span>

> <span data-ttu-id="b13dc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b13dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b13dc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b13dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b13dc-106">要对特定服务执行的 VPN 操作。</span><span class="sxs-lookup"><span data-stu-id="b13dc-106">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="b13dc-107">成员</span><span class="sxs-lookup"><span data-stu-id="b13dc-107">Members</span></span>
|<span data-ttu-id="b13dc-108">成员</span><span class="sxs-lookup"><span data-stu-id="b13dc-108">Member</span></span>|<span data-ttu-id="b13dc-109">值</span><span class="sxs-lookup"><span data-stu-id="b13dc-109">Value</span></span>|<span data-ttu-id="b13dc-110">说明</span><span class="sxs-lookup"><span data-stu-id="b13dc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b13dc-111">forceTrafficViaVPN</span><span class="sxs-lookup"><span data-stu-id="b13dc-111">forceTrafficViaVPN</span></span>|<span data-ttu-id="b13dc-112">0</span><span class="sxs-lookup"><span data-stu-id="b13dc-112">0</span></span>|<span data-ttu-id="b13dc-113">使来自该服务的所有流量都通过 VPN</span><span class="sxs-lookup"><span data-stu-id="b13dc-113">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="b13dc-114">allowTrafficOutside</span><span class="sxs-lookup"><span data-stu-id="b13dc-114">allowTrafficOutside</span></span>|<span data-ttu-id="b13dc-115">1</span><span class="sxs-lookup"><span data-stu-id="b13dc-115">1</span></span>|<span data-ttu-id="b13dc-116">允许 VPN 外部的服务</span><span class="sxs-lookup"><span data-stu-id="b13dc-116">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="b13dc-117">dropTraffic</span><span class="sxs-lookup"><span data-stu-id="b13dc-117">dropTraffic</span></span>|<span data-ttu-id="b13dc-118">双面</span><span class="sxs-lookup"><span data-stu-id="b13dc-118">2</span></span>|<span data-ttu-id="b13dc-119">从服务中删除所有流量</span><span class="sxs-lookup"><span data-stu-id="b13dc-119">Drop all traffic from the service</span></span>|



