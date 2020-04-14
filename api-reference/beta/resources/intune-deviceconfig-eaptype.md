---
title: eapType 枚举类型
description: 可扩展的身份验证协议（EAP）配置类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2508834aed066e6b9495624b872e7eeba0fdb22b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469123"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="5c9b1-103">eapType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5c9b1-103">eapType enum type</span></span>

<span data-ttu-id="5c9b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c9b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c9b1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c9b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c9b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c9b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c9b1-107">可扩展的身份验证协议（EAP）配置类型。</span><span class="sxs-lookup"><span data-stu-id="5c9b1-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>

## <a name="members"></a><span data-ttu-id="5c9b1-108">成员</span><span class="sxs-lookup"><span data-stu-id="5c9b1-108">Members</span></span>
|<span data-ttu-id="5c9b1-109">成员</span><span class="sxs-lookup"><span data-stu-id="5c9b1-109">Member</span></span>|<span data-ttu-id="5c9b1-110">值</span><span class="sxs-lookup"><span data-stu-id="5c9b1-110">Value</span></span>|<span data-ttu-id="5c9b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="5c9b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c9b1-112">eapTls</span><span class="sxs-lookup"><span data-stu-id="5c9b1-112">eapTls</span></span>|<span data-ttu-id="5c9b1-113">13</span><span class="sxs-lookup"><span data-stu-id="5c9b1-113">13</span></span>|<span data-ttu-id="5c9b1-114">EAP-传输层安全性（EAP-TLS）。</span><span class="sxs-lookup"><span data-stu-id="5c9b1-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="5c9b1-115">超越</span><span class="sxs-lookup"><span data-stu-id="5c9b1-115">leap</span></span>|<span data-ttu-id="5c9b1-116">17 </span><span class="sxs-lookup"><span data-stu-id="5c9b1-116">17</span></span>|<span data-ttu-id="5c9b1-117">轻型可扩展身份验证协议（LEAP）。</span><span class="sxs-lookup"><span data-stu-id="5c9b1-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="5c9b1-118">eapSim</span><span class="sxs-lookup"><span data-stu-id="5c9b1-118">eapSim</span></span>|<span data-ttu-id="5c9b1-119">18 </span><span class="sxs-lookup"><span data-stu-id="5c9b1-119">18</span></span>|<span data-ttu-id="5c9b1-120">适用于 GSM 订阅者标识模块（EAP-SIM）的 EAP。</span><span class="sxs-lookup"><span data-stu-id="5c9b1-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="5c9b1-121">eapTtls</span><span class="sxs-lookup"><span data-stu-id="5c9b1-121">eapTtls</span></span>|<span data-ttu-id="5c9b1-122">不足</span><span class="sxs-lookup"><span data-stu-id="5c9b1-122">21</span></span>|<span data-ttu-id="5c9b1-123">EAP-隧道传输层安全性（EAP-TTLS）。</span><span class="sxs-lookup"><span data-stu-id="5c9b1-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="5c9b1-124">peap</span><span class="sxs-lookup"><span data-stu-id="5c9b1-124">peap</span></span>|<span data-ttu-id="5c9b1-125">word</span><span class="sxs-lookup"><span data-stu-id="5c9b1-125">25</span></span>|<span data-ttu-id="5c9b1-126">受保护的可扩展身份验证协议（PEAP）。</span><span class="sxs-lookup"><span data-stu-id="5c9b1-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="5c9b1-127">eapFast</span><span class="sxs-lookup"><span data-stu-id="5c9b1-127">eapFast</span></span>|<span data-ttu-id="5c9b1-128">43</span><span class="sxs-lookup"><span data-stu-id="5c9b1-128">43</span></span>|<span data-ttu-id="5c9b1-129">通过安全隧道进行 EAP-灵活的身份验证（EAP-FAST）。</span><span class="sxs-lookup"><span data-stu-id="5c9b1-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|



