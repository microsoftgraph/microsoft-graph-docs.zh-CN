---
title: vpnTunnelConfigurationType 枚举类型
description: 将向 VPN 客户端提供的用于配置的隧道的类型
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d60d8fdd812fe18a5010683ddc0d1ef6cd8fbf06
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358928"
---
# <a name="vpntunnelconfigurationtype-enum-type"></a><span data-ttu-id="7da55-103">vpnTunnelConfigurationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7da55-103">vpnTunnelConfigurationType enum type</span></span>

<span data-ttu-id="7da55-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7da55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7da55-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7da55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7da55-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7da55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7da55-107">将向 VPN 客户端提供的用于配置的隧道的类型</span><span class="sxs-lookup"><span data-stu-id="7da55-107">The type of tunnels that will be present to the VPN client for configuration</span></span>

## <a name="members"></a><span data-ttu-id="7da55-108">成员</span><span class="sxs-lookup"><span data-stu-id="7da55-108">Members</span></span>
|<span data-ttu-id="7da55-109">成员</span><span class="sxs-lookup"><span data-stu-id="7da55-109">Member</span></span>|<span data-ttu-id="7da55-110">值</span><span class="sxs-lookup"><span data-stu-id="7da55-110">Value</span></span>|<span data-ttu-id="7da55-111">说明</span><span class="sxs-lookup"><span data-stu-id="7da55-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7da55-112">wifiAndCellular</span><span class="sxs-lookup"><span data-stu-id="7da55-112">wifiAndCellular</span></span>|<span data-ttu-id="7da55-113">0</span><span class="sxs-lookup"><span data-stu-id="7da55-113">0</span></span>|<span data-ttu-id="7da55-114">WiFi 和蜂窝隧道</span><span class="sxs-lookup"><span data-stu-id="7da55-114">WiFi and Cellular Tunnels</span></span>|
|<span data-ttu-id="7da55-115">蜂窝</span><span class="sxs-lookup"><span data-stu-id="7da55-115">cellular</span></span>|<span data-ttu-id="7da55-116">1</span><span class="sxs-lookup"><span data-stu-id="7da55-116">1</span></span>|<span data-ttu-id="7da55-117">仅蜂窝隧道</span><span class="sxs-lookup"><span data-stu-id="7da55-117">Cellular Tunnel Only</span></span>|
|<span data-ttu-id="7da55-118">wifi</span><span class="sxs-lookup"><span data-stu-id="7da55-118">wifi</span></span>|<span data-ttu-id="7da55-119">双面</span><span class="sxs-lookup"><span data-stu-id="7da55-119">2</span></span>|<span data-ttu-id="7da55-120">仅 WiFi 隧道</span><span class="sxs-lookup"><span data-stu-id="7da55-120">WiFi Tunnel Only</span></span>|



