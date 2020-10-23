---
title: eapType 枚举类型
description: 可扩展的身份验证协议 (EAP) 配置类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0d67147c281805e6d626f3f5e12fb5346ca90356
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48712027"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="b9dc9-103">eapType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b9dc9-103">eapType enum type</span></span>

<span data-ttu-id="b9dc9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9dc9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9dc9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9dc9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9dc9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9dc9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9dc9-107">可扩展的身份验证协议 (EAP) 配置类型。</span><span class="sxs-lookup"><span data-stu-id="b9dc9-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>

## <a name="members"></a><span data-ttu-id="b9dc9-108">成员</span><span class="sxs-lookup"><span data-stu-id="b9dc9-108">Members</span></span>
|<span data-ttu-id="b9dc9-109">成员</span><span class="sxs-lookup"><span data-stu-id="b9dc9-109">Member</span></span>|<span data-ttu-id="b9dc9-110">值</span><span class="sxs-lookup"><span data-stu-id="b9dc9-110">Value</span></span>|<span data-ttu-id="b9dc9-111">说明</span><span class="sxs-lookup"><span data-stu-id="b9dc9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9dc9-112">eapTls</span><span class="sxs-lookup"><span data-stu-id="b9dc9-112">eapTls</span></span>|<span data-ttu-id="b9dc9-113">13 </span><span class="sxs-lookup"><span data-stu-id="b9dc9-113">13</span></span>|<span data-ttu-id="b9dc9-114">EAP-Transport (EAP-TLS) 的层安全性。</span><span class="sxs-lookup"><span data-stu-id="b9dc9-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="b9dc9-115">超越</span><span class="sxs-lookup"><span data-stu-id="b9dc9-115">leap</span></span>|<span data-ttu-id="b9dc9-116">17 </span><span class="sxs-lookup"><span data-stu-id="b9dc9-116">17</span></span>|<span data-ttu-id="b9dc9-117"> (LEAP) 的轻型可扩展身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="b9dc9-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="b9dc9-118">eapSim</span><span class="sxs-lookup"><span data-stu-id="b9dc9-118">eapSim</span></span>|<span data-ttu-id="b9dc9-119">18 </span><span class="sxs-lookup"><span data-stu-id="b9dc9-119">18</span></span>|<span data-ttu-id="b9dc9-120">适用于 GSM 订阅者标识模块 (EAP-SIM) 的 EAP。</span><span class="sxs-lookup"><span data-stu-id="b9dc9-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="b9dc9-121">eapTtls</span><span class="sxs-lookup"><span data-stu-id="b9dc9-121">eapTtls</span></span>|<span data-ttu-id="b9dc9-122"> 21</span><span class="sxs-lookup"><span data-stu-id="b9dc9-122">21</span></span>|<span data-ttu-id="b9dc9-123">EAP-Tunneled (EAP-TTLS) 的传输层安全性。</span><span class="sxs-lookup"><span data-stu-id="b9dc9-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="b9dc9-124">peap</span><span class="sxs-lookup"><span data-stu-id="b9dc9-124">peap</span></span>|<span data-ttu-id="b9dc9-125">word</span><span class="sxs-lookup"><span data-stu-id="b9dc9-125">25</span></span>|<span data-ttu-id="b9dc9-126"> (PEAP) 的受保护的可扩展身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="b9dc9-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="b9dc9-127">eapFast</span><span class="sxs-lookup"><span data-stu-id="b9dc9-127">eapFast</span></span>|<span data-ttu-id="b9dc9-128">43</span><span class="sxs-lookup"><span data-stu-id="b9dc9-128">43</span></span>|<span data-ttu-id="b9dc9-129">通过安全隧道 (EAP-FAST) EAP-Flexible 身份验证。</span><span class="sxs-lookup"><span data-stu-id="b9dc9-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|





