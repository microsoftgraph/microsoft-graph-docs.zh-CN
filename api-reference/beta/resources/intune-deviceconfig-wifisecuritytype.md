---
title: wiFiSecurityType 枚举类型
description: Wi-fi 安全类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85c317706bb953fdeef202e4df9ec114944a7630
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944437"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="1133c-103">wiFiSecurityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1133c-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="1133c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1133c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1133c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1133c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1133c-106">Wi-fi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="1133c-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="1133c-107">成员</span><span class="sxs-lookup"><span data-stu-id="1133c-107">Members</span></span>
|<span data-ttu-id="1133c-108">成员</span><span class="sxs-lookup"><span data-stu-id="1133c-108">Member</span></span>|<span data-ttu-id="1133c-109">值</span><span class="sxs-lookup"><span data-stu-id="1133c-109">Value</span></span>|<span data-ttu-id="1133c-110">说明</span><span class="sxs-lookup"><span data-stu-id="1133c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1133c-111">open</span><span class="sxs-lookup"><span data-stu-id="1133c-111">open</span></span>|<span data-ttu-id="1133c-112">0</span><span class="sxs-lookup"><span data-stu-id="1133c-112">0</span></span>|<span data-ttu-id="1133c-113">打开 (无身份验证)。</span><span class="sxs-lookup"><span data-stu-id="1133c-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="1133c-114">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="1133c-114">wpaPersonal</span></span>|<span data-ttu-id="1133c-115">1</span><span class="sxs-lookup"><span data-stu-id="1133c-115">1</span></span>|<span data-ttu-id="1133c-116">WPA-个人版。</span><span class="sxs-lookup"><span data-stu-id="1133c-116">WPA-Personal.</span></span>|
|<span data-ttu-id="1133c-117">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="1133c-117">wpaEnterprise</span></span>|<span data-ttu-id="1133c-118">双面</span><span class="sxs-lookup"><span data-stu-id="1133c-118">2</span></span>|<span data-ttu-id="1133c-119">WPA-企业。</span><span class="sxs-lookup"><span data-stu-id="1133c-119">WPA-Enterprise.</span></span> <span data-ttu-id="1133c-120">必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="1133c-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="1133c-121">wep</span><span class="sxs-lookup"><span data-stu-id="1133c-121">wep</span></span>|<span data-ttu-id="1133c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="1133c-122">3</span></span>|<span data-ttu-id="1133c-123">WEP 加密。</span><span class="sxs-lookup"><span data-stu-id="1133c-123">WEP Encryption.</span></span>|
|<span data-ttu-id="1133c-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="1133c-124">wpa2Personal</span></span>|<span data-ttu-id="1133c-125">4</span><span class="sxs-lookup"><span data-stu-id="1133c-125">4</span></span>|<span data-ttu-id="1133c-126">WPA2-个人。</span><span class="sxs-lookup"><span data-stu-id="1133c-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="1133c-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="1133c-127">wpa2Enterprise</span></span>|<span data-ttu-id="1133c-128">5</span><span class="sxs-lookup"><span data-stu-id="1133c-128">5</span></span>|<span data-ttu-id="1133c-129">WPA2-企业。</span><span class="sxs-lookup"><span data-stu-id="1133c-129">WPA2-Enterprise.</span></span> <span data-ttu-id="1133c-130">必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="1133c-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




