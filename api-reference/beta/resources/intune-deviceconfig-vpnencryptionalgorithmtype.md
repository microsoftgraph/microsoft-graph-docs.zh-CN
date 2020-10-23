---
title: vpnEncryptionAlgorithmType 枚举类型
description: VPN 安全关联加密算法的类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 420dff0b05cae2bb403b7f8746063fc3417c4a4f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728368"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="41c15-103">vpnEncryptionAlgorithmType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="41c15-103">vpnEncryptionAlgorithmType enum type</span></span>

<span data-ttu-id="41c15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41c15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41c15-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41c15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41c15-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41c15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41c15-107">VPN 安全关联加密算法的类型</span><span class="sxs-lookup"><span data-stu-id="41c15-107">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="41c15-108">成员</span><span class="sxs-lookup"><span data-stu-id="41c15-108">Members</span></span>
|<span data-ttu-id="41c15-109">成员</span><span class="sxs-lookup"><span data-stu-id="41c15-109">Member</span></span>|<span data-ttu-id="41c15-110">值</span><span class="sxs-lookup"><span data-stu-id="41c15-110">Value</span></span>|<span data-ttu-id="41c15-111">说明</span><span class="sxs-lookup"><span data-stu-id="41c15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41c15-112">aes256</span><span class="sxs-lookup"><span data-stu-id="41c15-112">aes256</span></span>|<span data-ttu-id="41c15-113">0</span><span class="sxs-lookup"><span data-stu-id="41c15-113">0</span></span>|<span data-ttu-id="41c15-114">AES-256</span><span class="sxs-lookup"><span data-stu-id="41c15-114">AES-256</span></span>|
|<span data-ttu-id="41c15-115">des</span><span class="sxs-lookup"><span data-stu-id="41c15-115">des</span></span>|<span data-ttu-id="41c15-116">1</span><span class="sxs-lookup"><span data-stu-id="41c15-116">1</span></span>|<span data-ttu-id="41c15-117">DES</span><span class="sxs-lookup"><span data-stu-id="41c15-117">DES</span></span>|
|<span data-ttu-id="41c15-118">tripleDes</span><span class="sxs-lookup"><span data-stu-id="41c15-118">tripleDes</span></span>|<span data-ttu-id="41c15-119">双面</span><span class="sxs-lookup"><span data-stu-id="41c15-119">2</span></span>|<span data-ttu-id="41c15-120">3DES</span><span class="sxs-lookup"><span data-stu-id="41c15-120">3DES</span></span>|
|<span data-ttu-id="41c15-121">aes128-cts-hmac-sha1</span><span class="sxs-lookup"><span data-stu-id="41c15-121">aes128</span></span>|<span data-ttu-id="41c15-122">第三章</span><span class="sxs-lookup"><span data-stu-id="41c15-122">3</span></span>|<span data-ttu-id="41c15-123">AES-128</span><span class="sxs-lookup"><span data-stu-id="41c15-123">AES-128</span></span>|
|<span data-ttu-id="41c15-124">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="41c15-124">aes128Gcm</span></span>|<span data-ttu-id="41c15-125">4 </span><span class="sxs-lookup"><span data-stu-id="41c15-125">4</span></span>|<span data-ttu-id="41c15-126">AES-128-GCM (16-八进制 ICV) </span><span class="sxs-lookup"><span data-stu-id="41c15-126">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="41c15-127">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="41c15-127">aes256Gcm</span></span>|<span data-ttu-id="41c15-128">5 </span><span class="sxs-lookup"><span data-stu-id="41c15-128">5</span></span>|<span data-ttu-id="41c15-129">AES-256-GCM (16-八进制 ICV) </span><span class="sxs-lookup"><span data-stu-id="41c15-129">AES-256-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="41c15-130">aes192</span><span class="sxs-lookup"><span data-stu-id="41c15-130">aes192</span></span>|<span data-ttu-id="41c15-131">6 </span><span class="sxs-lookup"><span data-stu-id="41c15-131">6</span></span>|<span data-ttu-id="41c15-132">AES-192</span><span class="sxs-lookup"><span data-stu-id="41c15-132">AES-192</span></span>|
|<span data-ttu-id="41c15-133">aes192Gcm</span><span class="sxs-lookup"><span data-stu-id="41c15-133">aes192Gcm</span></span>|<span data-ttu-id="41c15-134">7 </span><span class="sxs-lookup"><span data-stu-id="41c15-134">7</span></span>|<span data-ttu-id="41c15-135">AES-192-GCM</span><span class="sxs-lookup"><span data-stu-id="41c15-135">AES-192-GCM</span></span>|





