---
title: androidWiFiSecurityType 枚举类型
description: 适用于 Android 的 wlan 安全类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1bbeec9421337b6af898f97f0f53e64cb0c45d7a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796683"
---
# <a name="androidwifisecuritytype-enum-type"></a><span data-ttu-id="df12d-103">androidWiFiSecurityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="df12d-103">androidWiFiSecurityType enum type</span></span>

> <span data-ttu-id="df12d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df12d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df12d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df12d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df12d-106">适用于 Android 的 wlan 安全类型。</span><span class="sxs-lookup"><span data-stu-id="df12d-106">Wi-Fi Security Types for Android.</span></span>

## <a name="members"></a><span data-ttu-id="df12d-107">成员</span><span class="sxs-lookup"><span data-stu-id="df12d-107">Members</span></span>
|<span data-ttu-id="df12d-108">成员</span><span class="sxs-lookup"><span data-stu-id="df12d-108">Member</span></span>|<span data-ttu-id="df12d-109">值</span><span class="sxs-lookup"><span data-stu-id="df12d-109">Value</span></span>|<span data-ttu-id="df12d-110">说明</span><span class="sxs-lookup"><span data-stu-id="df12d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df12d-111">open</span><span class="sxs-lookup"><span data-stu-id="df12d-111">open</span></span>|<span data-ttu-id="df12d-112">0</span><span class="sxs-lookup"><span data-stu-id="df12d-112">0</span></span>|<span data-ttu-id="df12d-113">打开（无身份验证）。</span><span class="sxs-lookup"><span data-stu-id="df12d-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="df12d-114">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="df12d-114">wpaEnterprise</span></span>|<span data-ttu-id="df12d-115">1</span><span class="sxs-lookup"><span data-stu-id="df12d-115">1</span></span>|<span data-ttu-id="df12d-116">WPA-企业。</span><span class="sxs-lookup"><span data-stu-id="df12d-116">WPA-Enterprise.</span></span> <span data-ttu-id="df12d-117">必须使用 AndroidEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="df12d-117">Must use AndroidEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="df12d-118">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="df12d-118">wpa2Enterprise</span></span>|<span data-ttu-id="df12d-119">双面</span><span class="sxs-lookup"><span data-stu-id="df12d-119">2</span></span>|<span data-ttu-id="df12d-120">WPA2-企业。</span><span class="sxs-lookup"><span data-stu-id="df12d-120">WPA2-Enterprise.</span></span> <span data-ttu-id="df12d-121">必须使用 AndroidEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="df12d-121">Must use AndroidEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|



