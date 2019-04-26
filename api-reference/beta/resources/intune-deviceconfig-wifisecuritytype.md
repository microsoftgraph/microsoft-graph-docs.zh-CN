---
title: wiFiSecurityType 枚举类型
description: wi-fi 安全类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9144a5761691b0a50e40370b1f4d2d08967f2c28
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554840"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="37a0e-103">wiFiSecurityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="37a0e-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="37a0e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="37a0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37a0e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37a0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37a0e-106">wi-fi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="37a0e-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="37a0e-107">成员</span><span class="sxs-lookup"><span data-stu-id="37a0e-107">Members</span></span>
|<span data-ttu-id="37a0e-108">成员</span><span class="sxs-lookup"><span data-stu-id="37a0e-108">Member</span></span>|<span data-ttu-id="37a0e-109">值</span><span class="sxs-lookup"><span data-stu-id="37a0e-109">Value</span></span>|<span data-ttu-id="37a0e-110">说明</span><span class="sxs-lookup"><span data-stu-id="37a0e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37a0e-111">open</span><span class="sxs-lookup"><span data-stu-id="37a0e-111">open</span></span>|<span data-ttu-id="37a0e-112">0</span><span class="sxs-lookup"><span data-stu-id="37a0e-112">0</span></span>|<span data-ttu-id="37a0e-113">打开 (无身份验证)。</span><span class="sxs-lookup"><span data-stu-id="37a0e-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="37a0e-114">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="37a0e-114">wpaPersonal</span></span>|<span data-ttu-id="37a0e-115">1</span><span class="sxs-lookup"><span data-stu-id="37a0e-115">1</span></span>|<span data-ttu-id="37a0e-116">WPA-个人版。</span><span class="sxs-lookup"><span data-stu-id="37a0e-116">WPA-Personal.</span></span>|
|<span data-ttu-id="37a0e-117">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="37a0e-117">wpaEnterprise</span></span>|<span data-ttu-id="37a0e-118">2 </span><span class="sxs-lookup"><span data-stu-id="37a0e-118">2</span></span>|<span data-ttu-id="37a0e-119">WPA-企业。</span><span class="sxs-lookup"><span data-stu-id="37a0e-119">WPA-Enterprise.</span></span> <span data-ttu-id="37a0e-120">必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="37a0e-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="37a0e-121">wep</span><span class="sxs-lookup"><span data-stu-id="37a0e-121">wep</span></span>|<span data-ttu-id="37a0e-122">3 </span><span class="sxs-lookup"><span data-stu-id="37a0e-122">3</span></span>|<span data-ttu-id="37a0e-123">WEP 加密。</span><span class="sxs-lookup"><span data-stu-id="37a0e-123">WEP Encryption.</span></span>|
|<span data-ttu-id="37a0e-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="37a0e-124">wpa2Personal</span></span>|<span data-ttu-id="37a0e-125">4 </span><span class="sxs-lookup"><span data-stu-id="37a0e-125">4</span></span>|<span data-ttu-id="37a0e-126">WPA2-个人。</span><span class="sxs-lookup"><span data-stu-id="37a0e-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="37a0e-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="37a0e-127">wpa2Enterprise</span></span>|<span data-ttu-id="37a0e-128">5 </span><span class="sxs-lookup"><span data-stu-id="37a0e-128">5</span></span>|<span data-ttu-id="37a0e-129">WPA2-企业。</span><span class="sxs-lookup"><span data-stu-id="37a0e-129">WPA2-Enterprise.</span></span> <span data-ttu-id="37a0e-130">必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="37a0e-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





