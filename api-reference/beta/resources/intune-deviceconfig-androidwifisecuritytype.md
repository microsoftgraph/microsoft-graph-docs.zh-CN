---
title: androidWiFiSecurityType 枚举类型
description: 适用于 Android 的 Wi-Fi 安全类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 78f910f7b93d33fcd86ad658e38ad2fa923c7835
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283929"
---
# <a name="androidwifisecuritytype-enum-type"></a><span data-ttu-id="6ffea-103">androidWiFiSecurityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6ffea-103">androidWiFiSecurityType enum type</span></span>

<span data-ttu-id="6ffea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ffea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ffea-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ffea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ffea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ffea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ffea-107">适用于 Android 的 Wi-Fi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="6ffea-107">Wi-Fi Security Types for Android.</span></span>

## <a name="members"></a><span data-ttu-id="6ffea-108">成员</span><span class="sxs-lookup"><span data-stu-id="6ffea-108">Members</span></span>
|<span data-ttu-id="6ffea-109">成员</span><span class="sxs-lookup"><span data-stu-id="6ffea-109">Member</span></span>|<span data-ttu-id="6ffea-110">值</span><span class="sxs-lookup"><span data-stu-id="6ffea-110">Value</span></span>|<span data-ttu-id="6ffea-111">Description</span><span class="sxs-lookup"><span data-stu-id="6ffea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ffea-112">open</span><span class="sxs-lookup"><span data-stu-id="6ffea-112">open</span></span>|<span data-ttu-id="6ffea-113">0</span><span class="sxs-lookup"><span data-stu-id="6ffea-113">0</span></span>|<span data-ttu-id="6ffea-114">打开 (不进行身份验证) 。</span><span class="sxs-lookup"><span data-stu-id="6ffea-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="6ffea-115">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="6ffea-115">wpaEnterprise</span></span>|<span data-ttu-id="6ffea-116">1</span><span class="sxs-lookup"><span data-stu-id="6ffea-116">1</span></span>|<span data-ttu-id="6ffea-117">WPA-企业。</span><span class="sxs-lookup"><span data-stu-id="6ffea-117">WPA-Enterprise.</span></span> <span data-ttu-id="6ffea-118">必须使用 AndroidEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="6ffea-118">Must use AndroidEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="6ffea-119">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="6ffea-119">wpa2Enterprise</span></span>|<span data-ttu-id="6ffea-120">双面</span><span class="sxs-lookup"><span data-stu-id="6ffea-120">2</span></span>|<span data-ttu-id="6ffea-121">WPA2-企业。</span><span class="sxs-lookup"><span data-stu-id="6ffea-121">WPA2-Enterprise.</span></span> <span data-ttu-id="6ffea-122">必须使用 AndroidEnterpriseWifiConfiguration 类型配置企业选项。</span><span class="sxs-lookup"><span data-stu-id="6ffea-122">Must use AndroidEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|




