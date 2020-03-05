---
title: vpnServiceExceptionAction 枚举类型
description: 要对特定服务执行的 VPN 操作。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a7c202c404d9d1db16e328f9c7d4c220ddd481e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525738"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="6f1be-103">vpnServiceExceptionAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6f1be-103">vpnServiceExceptionAction enum type</span></span>

<span data-ttu-id="6f1be-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6f1be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f1be-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6f1be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f1be-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f1be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f1be-107">要对特定服务执行的 VPN 操作。</span><span class="sxs-lookup"><span data-stu-id="6f1be-107">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="6f1be-108">成员</span><span class="sxs-lookup"><span data-stu-id="6f1be-108">Members</span></span>
|<span data-ttu-id="6f1be-109">成员</span><span class="sxs-lookup"><span data-stu-id="6f1be-109">Member</span></span>|<span data-ttu-id="6f1be-110">值</span><span class="sxs-lookup"><span data-stu-id="6f1be-110">Value</span></span>|<span data-ttu-id="6f1be-111">说明</span><span class="sxs-lookup"><span data-stu-id="6f1be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f1be-112">forceTrafficViaVPN</span><span class="sxs-lookup"><span data-stu-id="6f1be-112">forceTrafficViaVPN</span></span>|<span data-ttu-id="6f1be-113">0</span><span class="sxs-lookup"><span data-stu-id="6f1be-113">0</span></span>|<span data-ttu-id="6f1be-114">使来自该服务的所有流量都通过 VPN</span><span class="sxs-lookup"><span data-stu-id="6f1be-114">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="6f1be-115">allowTrafficOutside</span><span class="sxs-lookup"><span data-stu-id="6f1be-115">allowTrafficOutside</span></span>|<span data-ttu-id="6f1be-116">1 </span><span class="sxs-lookup"><span data-stu-id="6f1be-116">1</span></span>|<span data-ttu-id="6f1be-117">允许 VPN 外部的服务</span><span class="sxs-lookup"><span data-stu-id="6f1be-117">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="6f1be-118">dropTraffic</span><span class="sxs-lookup"><span data-stu-id="6f1be-118">dropTraffic</span></span>|<span data-ttu-id="6f1be-119">2 </span><span class="sxs-lookup"><span data-stu-id="6f1be-119">2</span></span>|<span data-ttu-id="6f1be-120">从服务中删除所有流量</span><span class="sxs-lookup"><span data-stu-id="6f1be-120">Drop all traffic from the service</span></span>|



