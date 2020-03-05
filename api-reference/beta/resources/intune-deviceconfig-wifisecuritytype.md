---
title: wiFiSecurityType 枚举类型
description: Wi-fi 安全类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 33d7116bb686945672d96d20035d18ed1df3ee9e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525703"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="4f8c2-103">wiFiSecurityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4f8c2-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="4f8c2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4f8c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f8c2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f8c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f8c2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f8c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f8c2-107">Wi-fi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="4f8c2-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="4f8c2-108">成员</span><span class="sxs-lookup"><span data-stu-id="4f8c2-108">Members</span></span>
|<span data-ttu-id="4f8c2-109">成员</span><span class="sxs-lookup"><span data-stu-id="4f8c2-109">Member</span></span>|<span data-ttu-id="4f8c2-110">值</span><span class="sxs-lookup"><span data-stu-id="4f8c2-110">Value</span></span>|<span data-ttu-id="4f8c2-111">说明</span><span class="sxs-lookup"><span data-stu-id="4f8c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f8c2-112">open</span><span class="sxs-lookup"><span data-stu-id="4f8c2-112">open</span></span>|<span data-ttu-id="4f8c2-113">0</span><span class="sxs-lookup"><span data-stu-id="4f8c2-113">0</span></span>|<span data-ttu-id="4f8c2-114">打开（无身份验证）。</span><span class="sxs-lookup"><span data-stu-id="4f8c2-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="4f8c2-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="4f8c2-115">wpaPersonal</span></span>|<span data-ttu-id="4f8c2-116">1 </span><span class="sxs-lookup"><span data-stu-id="4f8c2-116">1</span></span>|<span data-ttu-id="4f8c2-117">WPA-个人版。</span><span class="sxs-lookup"><span data-stu-id="4f8c2-117">WPA-Personal.</span></span>|
|<span data-ttu-id="4f8c2-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="4f8c2-118">wpaEnterprise</span></span>|<span data-ttu-id="4f8c2-119">2 </span><span class="sxs-lookup"><span data-stu-id="4f8c2-119">2</span></span>|<span data-ttu-id="4f8c2-120">WPA-企业。</span><span class="sxs-lookup"><span data-stu-id="4f8c2-120">WPA-Enterprise.</span></span> <span data-ttu-id="4f8c2-121">必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="4f8c2-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="4f8c2-122">wep</span><span class="sxs-lookup"><span data-stu-id="4f8c2-122">wep</span></span>|<span data-ttu-id="4f8c2-123">3 </span><span class="sxs-lookup"><span data-stu-id="4f8c2-123">3</span></span>|<span data-ttu-id="4f8c2-124">WEP 加密。</span><span class="sxs-lookup"><span data-stu-id="4f8c2-124">WEP Encryption.</span></span>|
|<span data-ttu-id="4f8c2-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="4f8c2-125">wpa2Personal</span></span>|<span data-ttu-id="4f8c2-126">4 </span><span class="sxs-lookup"><span data-stu-id="4f8c2-126">4</span></span>|<span data-ttu-id="4f8c2-127">WPA2-个人。</span><span class="sxs-lookup"><span data-stu-id="4f8c2-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="4f8c2-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="4f8c2-128">wpa2Enterprise</span></span>|<span data-ttu-id="4f8c2-129">5 </span><span class="sxs-lookup"><span data-stu-id="4f8c2-129">5</span></span>|<span data-ttu-id="4f8c2-130">WPA2-企业。</span><span class="sxs-lookup"><span data-stu-id="4f8c2-130">WPA2-Enterprise.</span></span> <span data-ttu-id="4f8c2-131">必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="4f8c2-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|



