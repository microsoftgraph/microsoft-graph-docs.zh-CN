---
title: androidDeviceOwnerWiFiSecurityType 枚举类型
description: Android 设备所有者的 wi-fi 安全类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 725a786de238d8965507dc590cfd200fd91b13e7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983748"
---
# <a name="androiddeviceownerwifisecuritytype-enum-type"></a><span data-ttu-id="bb210-103">androidDeviceOwnerWiFiSecurityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bb210-103">androidDeviceOwnerWiFiSecurityType enum type</span></span>

> <span data-ttu-id="bb210-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb210-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb210-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb210-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb210-106">Android 设备所有者的 wi-fi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="bb210-106">Wi-Fi Security Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="bb210-107">成员</span><span class="sxs-lookup"><span data-stu-id="bb210-107">Members</span></span>
|<span data-ttu-id="bb210-108">成员</span><span class="sxs-lookup"><span data-stu-id="bb210-108">Member</span></span>|<span data-ttu-id="bb210-109">值</span><span class="sxs-lookup"><span data-stu-id="bb210-109">Value</span></span>|<span data-ttu-id="bb210-110">说明</span><span class="sxs-lookup"><span data-stu-id="bb210-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb210-111">open</span><span class="sxs-lookup"><span data-stu-id="bb210-111">open</span></span>|<span data-ttu-id="bb210-112">0</span><span class="sxs-lookup"><span data-stu-id="bb210-112">0</span></span>|<span data-ttu-id="bb210-113">打开 (无身份验证)。</span><span class="sxs-lookup"><span data-stu-id="bb210-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="bb210-114">wep</span><span class="sxs-lookup"><span data-stu-id="bb210-114">wep</span></span>|<span data-ttu-id="bb210-115">1</span><span class="sxs-lookup"><span data-stu-id="bb210-115">1</span></span>|<span data-ttu-id="bb210-116">WEP 加密。</span><span class="sxs-lookup"><span data-stu-id="bb210-116">WEP Encryption.</span></span>|
|<span data-ttu-id="bb210-117">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="bb210-117">wpaPersonal</span></span>|<span data-ttu-id="bb210-118">双面</span><span class="sxs-lookup"><span data-stu-id="bb210-118">2</span></span>|<span data-ttu-id="bb210-119">WPA-个人/WPA2-个人。</span><span class="sxs-lookup"><span data-stu-id="bb210-119">WPA-Personal/WPA2-Personal.</span></span>|
|<span data-ttu-id="bb210-120">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="bb210-120">wpaEnterprise</span></span>|<span data-ttu-id="bb210-121">4</span><span class="sxs-lookup"><span data-stu-id="bb210-121">4</span></span>|<span data-ttu-id="bb210-122">WPA-企业/WPA2-企业。</span><span class="sxs-lookup"><span data-stu-id="bb210-122">WPA-Enterprise/WPA2-Enterprise.</span></span> <span data-ttu-id="bb210-123">必须使用 AndroidDeviceOwnerEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="bb210-123">Must use AndroidDeviceOwnerEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|





