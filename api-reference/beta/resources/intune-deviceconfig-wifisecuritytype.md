---
title: wiFiSecurityType 枚举类型
description: Wi-Fi 安全类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e01faac094cd2ae040137b251d30006883388173
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732528"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="a9f0d-103">wiFiSecurityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a9f0d-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="a9f0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9f0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9f0d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9f0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9f0d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9f0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9f0d-107">Wi-Fi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="a9f0d-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="a9f0d-108">成员</span><span class="sxs-lookup"><span data-stu-id="a9f0d-108">Members</span></span>
|<span data-ttu-id="a9f0d-109">成员</span><span class="sxs-lookup"><span data-stu-id="a9f0d-109">Member</span></span>|<span data-ttu-id="a9f0d-110">值</span><span class="sxs-lookup"><span data-stu-id="a9f0d-110">Value</span></span>|<span data-ttu-id="a9f0d-111">说明</span><span class="sxs-lookup"><span data-stu-id="a9f0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f0d-112">open</span><span class="sxs-lookup"><span data-stu-id="a9f0d-112">open</span></span>|<span data-ttu-id="a9f0d-113">0</span><span class="sxs-lookup"><span data-stu-id="a9f0d-113">0</span></span>|<span data-ttu-id="a9f0d-114">打开 (不进行身份验证) 。</span><span class="sxs-lookup"><span data-stu-id="a9f0d-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="a9f0d-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="a9f0d-115">wpaPersonal</span></span>|<span data-ttu-id="a9f0d-116">1</span><span class="sxs-lookup"><span data-stu-id="a9f0d-116">1</span></span>|<span data-ttu-id="a9f0d-117">WPA-个人版。</span><span class="sxs-lookup"><span data-stu-id="a9f0d-117">WPA-Personal.</span></span>|
|<span data-ttu-id="a9f0d-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="a9f0d-118">wpaEnterprise</span></span>|<span data-ttu-id="a9f0d-119">双面</span><span class="sxs-lookup"><span data-stu-id="a9f0d-119">2</span></span>|<span data-ttu-id="a9f0d-120">WPA-企业。</span><span class="sxs-lookup"><span data-stu-id="a9f0d-120">WPA-Enterprise.</span></span> <span data-ttu-id="a9f0d-121">必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="a9f0d-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="a9f0d-122">wep</span><span class="sxs-lookup"><span data-stu-id="a9f0d-122">wep</span></span>|<span data-ttu-id="a9f0d-123">第三章</span><span class="sxs-lookup"><span data-stu-id="a9f0d-123">3</span></span>|<span data-ttu-id="a9f0d-124">WEP 加密。</span><span class="sxs-lookup"><span data-stu-id="a9f0d-124">WEP Encryption.</span></span>|
|<span data-ttu-id="a9f0d-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="a9f0d-125">wpa2Personal</span></span>|<span data-ttu-id="a9f0d-126">4 </span><span class="sxs-lookup"><span data-stu-id="a9f0d-126">4</span></span>|<span data-ttu-id="a9f0d-127">WPA2-个人。</span><span class="sxs-lookup"><span data-stu-id="a9f0d-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="a9f0d-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="a9f0d-128">wpa2Enterprise</span></span>|<span data-ttu-id="a9f0d-129">5 </span><span class="sxs-lookup"><span data-stu-id="a9f0d-129">5</span></span>|<span data-ttu-id="a9f0d-130">WPA2-企业。</span><span class="sxs-lookup"><span data-stu-id="a9f0d-130">WPA2-Enterprise.</span></span> <span data-ttu-id="a9f0d-131">必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="a9f0d-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





