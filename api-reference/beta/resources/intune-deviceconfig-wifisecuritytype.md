---
title: wiFiSecurityType 枚举类型
description: Wi-fi 安全类型。
author: tfitzmac
ms.openlocfilehash: 291bc3660971a90ea113959368542e715a86b570
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329188"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="7a763-103">wiFiSecurityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7a763-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="7a763-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7a763-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a763-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7a763-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a763-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7a763-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a763-107">Wi-fi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="7a763-107">Wi-Fi Security Types.</span></span>
## <a name="members"></a><span data-ttu-id="7a763-108">成员</span><span class="sxs-lookup"><span data-stu-id="7a763-108">Members</span></span>
|<span data-ttu-id="7a763-109">成员</span><span class="sxs-lookup"><span data-stu-id="7a763-109">Member</span></span>|<span data-ttu-id="7a763-110">值</span><span class="sxs-lookup"><span data-stu-id="7a763-110">Value</span></span>|<span data-ttu-id="7a763-111">说明</span><span class="sxs-lookup"><span data-stu-id="7a763-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a763-112">打开</span><span class="sxs-lookup"><span data-stu-id="7a763-112">open</span></span>|<span data-ttu-id="7a763-113">0</span><span class="sxs-lookup"><span data-stu-id="7a763-113">0</span></span>|<span data-ttu-id="7a763-114">打开 （无身份验证）。</span><span class="sxs-lookup"><span data-stu-id="7a763-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="7a763-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="7a763-115">wpaPersonal</span></span>|<span data-ttu-id="7a763-116">1</span><span class="sxs-lookup"><span data-stu-id="7a763-116">1</span></span>|<span data-ttu-id="7a763-117">WPA-个人。</span><span class="sxs-lookup"><span data-stu-id="7a763-117">WPA-Personal.</span></span>|
|<span data-ttu-id="7a763-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="7a763-118">wpaEnterprise</span></span>|<span data-ttu-id="7a763-119">2</span><span class="sxs-lookup"><span data-stu-id="7a763-119">2</span></span>|<span data-ttu-id="7a763-120">WPA-企业。</span><span class="sxs-lookup"><span data-stu-id="7a763-120">WPA-Enterprise.</span></span> <span data-ttu-id="7a763-121">必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="7a763-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="7a763-122">wep</span><span class="sxs-lookup"><span data-stu-id="7a763-122">wep</span></span>|<span data-ttu-id="7a763-123">3</span><span class="sxs-lookup"><span data-stu-id="7a763-123">3</span></span>|<span data-ttu-id="7a763-124">WEP 加密。</span><span class="sxs-lookup"><span data-stu-id="7a763-124">WEP Encryption.</span></span>|
|<span data-ttu-id="7a763-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="7a763-125">wpa2Personal</span></span>|<span data-ttu-id="7a763-126">4</span><span class="sxs-lookup"><span data-stu-id="7a763-126">4</span></span>|<span data-ttu-id="7a763-127">WPA2-个人。</span><span class="sxs-lookup"><span data-stu-id="7a763-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="7a763-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="7a763-128">wpa2Enterprise</span></span>|<span data-ttu-id="7a763-129">5</span><span class="sxs-lookup"><span data-stu-id="7a763-129">5</span></span>|<span data-ttu-id="7a763-130">WPA2-企业。</span><span class="sxs-lookup"><span data-stu-id="7a763-130">WPA2-Enterprise.</span></span> <span data-ttu-id="7a763-131">必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="7a763-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





