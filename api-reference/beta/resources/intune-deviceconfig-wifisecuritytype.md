---
title: wiFiSecurityType 枚举类型
description: Wi-fi 安全类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22dd7bf07e6355dd92f04461120e3afb142d6d9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048874"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="5778a-103">wiFiSecurityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5778a-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="5778a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5778a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5778a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5778a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5778a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5778a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5778a-107">Wi-fi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="5778a-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="5778a-108">成员</span><span class="sxs-lookup"><span data-stu-id="5778a-108">Members</span></span>
|<span data-ttu-id="5778a-109">成员</span><span class="sxs-lookup"><span data-stu-id="5778a-109">Member</span></span>|<span data-ttu-id="5778a-110">值</span><span class="sxs-lookup"><span data-stu-id="5778a-110">Value</span></span>|<span data-ttu-id="5778a-111">说明</span><span class="sxs-lookup"><span data-stu-id="5778a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5778a-112">open</span><span class="sxs-lookup"><span data-stu-id="5778a-112">open</span></span>|<span data-ttu-id="5778a-113">0</span><span class="sxs-lookup"><span data-stu-id="5778a-113">0</span></span>|<span data-ttu-id="5778a-114">打开 (不进行身份验证) 。</span><span class="sxs-lookup"><span data-stu-id="5778a-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="5778a-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="5778a-115">wpaPersonal</span></span>|<span data-ttu-id="5778a-116">1 </span><span class="sxs-lookup"><span data-stu-id="5778a-116">1</span></span>|<span data-ttu-id="5778a-117">WPA-个人版。</span><span class="sxs-lookup"><span data-stu-id="5778a-117">WPA-Personal.</span></span>|
|<span data-ttu-id="5778a-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="5778a-118">wpaEnterprise</span></span>|<span data-ttu-id="5778a-119">2 </span><span class="sxs-lookup"><span data-stu-id="5778a-119">2</span></span>|<span data-ttu-id="5778a-120">WPA-企业。</span><span class="sxs-lookup"><span data-stu-id="5778a-120">WPA-Enterprise.</span></span> <span data-ttu-id="5778a-121">必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="5778a-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="5778a-122">wep</span><span class="sxs-lookup"><span data-stu-id="5778a-122">wep</span></span>|<span data-ttu-id="5778a-123">第三章</span><span class="sxs-lookup"><span data-stu-id="5778a-123">3</span></span>|<span data-ttu-id="5778a-124">WEP 加密。</span><span class="sxs-lookup"><span data-stu-id="5778a-124">WEP Encryption.</span></span>|
|<span data-ttu-id="5778a-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="5778a-125">wpa2Personal</span></span>|<span data-ttu-id="5778a-126">4 </span><span class="sxs-lookup"><span data-stu-id="5778a-126">4</span></span>|<span data-ttu-id="5778a-127">WPA2-个人。</span><span class="sxs-lookup"><span data-stu-id="5778a-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="5778a-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="5778a-128">wpa2Enterprise</span></span>|<span data-ttu-id="5778a-129">5 </span><span class="sxs-lookup"><span data-stu-id="5778a-129">5</span></span>|<span data-ttu-id="5778a-130">WPA2-企业。</span><span class="sxs-lookup"><span data-stu-id="5778a-130">WPA2-Enterprise.</span></span> <span data-ttu-id="5778a-131">必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="5778a-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|






