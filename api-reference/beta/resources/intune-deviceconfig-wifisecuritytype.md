---
title: wiFiSecurityType 枚举类型
description: Wi-fi 安全类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 73724041c223d50d0030bf27b780d6b694792a16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422129"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="fd3c6-103">wiFiSecurityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fd3c6-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="fd3c6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fd3c6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd3c6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd3c6-107">Wi-fi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="fd3c6-108">成员</span><span class="sxs-lookup"><span data-stu-id="fd3c6-108">Members</span></span>
|<span data-ttu-id="fd3c6-109">成员</span><span class="sxs-lookup"><span data-stu-id="fd3c6-109">Member</span></span>|<span data-ttu-id="fd3c6-110">值</span><span class="sxs-lookup"><span data-stu-id="fd3c6-110">Value</span></span>|<span data-ttu-id="fd3c6-111">说明</span><span class="sxs-lookup"><span data-stu-id="fd3c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd3c6-112">打开</span><span class="sxs-lookup"><span data-stu-id="fd3c6-112">open</span></span>|<span data-ttu-id="fd3c6-113">0</span><span class="sxs-lookup"><span data-stu-id="fd3c6-113">0</span></span>|<span data-ttu-id="fd3c6-114">打开 （无身份验证）。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="fd3c6-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="fd3c6-115">wpaPersonal</span></span>|<span data-ttu-id="fd3c6-116">1</span><span class="sxs-lookup"><span data-stu-id="fd3c6-116">1</span></span>|<span data-ttu-id="fd3c6-117">WPA-个人。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-117">WPA-Personal.</span></span>|
|<span data-ttu-id="fd3c6-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="fd3c6-118">wpaEnterprise</span></span>|<span data-ttu-id="fd3c6-119">2</span><span class="sxs-lookup"><span data-stu-id="fd3c6-119">2</span></span>|<span data-ttu-id="fd3c6-120">WPA-企业。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-120">WPA-Enterprise.</span></span> <span data-ttu-id="fd3c6-121">必须使用 IOSEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="fd3c6-122">wep</span><span class="sxs-lookup"><span data-stu-id="fd3c6-122">wep</span></span>|<span data-ttu-id="fd3c6-123">3</span><span class="sxs-lookup"><span data-stu-id="fd3c6-123">3</span></span>|<span data-ttu-id="fd3c6-124">WEP 加密。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-124">WEP Encryption.</span></span>|
|<span data-ttu-id="fd3c6-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="fd3c6-125">wpa2Personal</span></span>|<span data-ttu-id="fd3c6-126">4</span><span class="sxs-lookup"><span data-stu-id="fd3c6-126">4</span></span>|<span data-ttu-id="fd3c6-127">WPA2-个人。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="fd3c6-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="fd3c6-128">wpa2Enterprise</span></span>|<span data-ttu-id="fd3c6-129">5</span><span class="sxs-lookup"><span data-stu-id="fd3c6-129">5</span></span>|<span data-ttu-id="fd3c6-130">WPA2-企业。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-130">WPA2-Enterprise.</span></span> <span data-ttu-id="fd3c6-131">必须使用 WindowsWifiEnterpriseEAPConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="fd3c6-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




