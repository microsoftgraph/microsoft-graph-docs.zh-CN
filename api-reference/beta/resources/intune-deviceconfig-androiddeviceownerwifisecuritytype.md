---
title: androidDeviceOwnerWiFiSecurityType 枚举类型
description: 适用于 Android 设备所有者的 Wi-Fi 安全类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 742c21c0358cab27050d75e94065bb788ceec6fa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294835"
---
# <a name="androiddeviceownerwifisecuritytype-enum-type"></a><span data-ttu-id="a0829-103">androidDeviceOwnerWiFiSecurityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a0829-103">androidDeviceOwnerWiFiSecurityType enum type</span></span>

<span data-ttu-id="a0829-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0829-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0829-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a0829-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0829-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a0829-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0829-107">适用于 Android 设备所有者的 Wi-Fi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="a0829-107">Wi-Fi Security Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="a0829-108">成员</span><span class="sxs-lookup"><span data-stu-id="a0829-108">Members</span></span>
|<span data-ttu-id="a0829-109">成员</span><span class="sxs-lookup"><span data-stu-id="a0829-109">Member</span></span>|<span data-ttu-id="a0829-110">值</span><span class="sxs-lookup"><span data-stu-id="a0829-110">Value</span></span>|<span data-ttu-id="a0829-111">Description</span><span class="sxs-lookup"><span data-stu-id="a0829-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0829-112">open</span><span class="sxs-lookup"><span data-stu-id="a0829-112">open</span></span>|<span data-ttu-id="a0829-113">0</span><span class="sxs-lookup"><span data-stu-id="a0829-113">0</span></span>|<span data-ttu-id="a0829-114">打开 (不进行身份验证) 。</span><span class="sxs-lookup"><span data-stu-id="a0829-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="a0829-115">wep</span><span class="sxs-lookup"><span data-stu-id="a0829-115">wep</span></span>|<span data-ttu-id="a0829-116">1</span><span class="sxs-lookup"><span data-stu-id="a0829-116">1</span></span>|<span data-ttu-id="a0829-117">WEP 加密。</span><span class="sxs-lookup"><span data-stu-id="a0829-117">WEP Encryption.</span></span>|
|<span data-ttu-id="a0829-118">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="a0829-118">wpaPersonal</span></span>|<span data-ttu-id="a0829-119">双面</span><span class="sxs-lookup"><span data-stu-id="a0829-119">2</span></span>|<span data-ttu-id="a0829-120">WPA-个人/WPA2-个人。</span><span class="sxs-lookup"><span data-stu-id="a0829-120">WPA-Personal/WPA2-Personal.</span></span>|
|<span data-ttu-id="a0829-121">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="a0829-121">wpaEnterprise</span></span>|<span data-ttu-id="a0829-122">4 </span><span class="sxs-lookup"><span data-stu-id="a0829-122">4</span></span>|<span data-ttu-id="a0829-123">WPA-企业/WPA2-企业。</span><span class="sxs-lookup"><span data-stu-id="a0829-123">WPA-Enterprise/WPA2-Enterprise.</span></span> <span data-ttu-id="a0829-124">必须使用 AndroidDeviceOwnerEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="a0829-124">Must use AndroidDeviceOwnerEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|




