---
title: vpnEncryptionAlgorithmType 枚举类型
description: VPN 安全关联加密算法的类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f7813f66781f0443c570198248349c1bb08716fd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299658"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="76f2c-103">vpnEncryptionAlgorithmType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="76f2c-103">vpnEncryptionAlgorithmType enum type</span></span>

<span data-ttu-id="76f2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76f2c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76f2c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76f2c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76f2c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76f2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76f2c-107">VPN 安全关联加密算法的类型</span><span class="sxs-lookup"><span data-stu-id="76f2c-107">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="76f2c-108">成员</span><span class="sxs-lookup"><span data-stu-id="76f2c-108">Members</span></span>
|<span data-ttu-id="76f2c-109">成员</span><span class="sxs-lookup"><span data-stu-id="76f2c-109">Member</span></span>|<span data-ttu-id="76f2c-110">值</span><span class="sxs-lookup"><span data-stu-id="76f2c-110">Value</span></span>|<span data-ttu-id="76f2c-111">Description</span><span class="sxs-lookup"><span data-stu-id="76f2c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76f2c-112">aes256</span><span class="sxs-lookup"><span data-stu-id="76f2c-112">aes256</span></span>|<span data-ttu-id="76f2c-113">0</span><span class="sxs-lookup"><span data-stu-id="76f2c-113">0</span></span>|<span data-ttu-id="76f2c-114">AES-256</span><span class="sxs-lookup"><span data-stu-id="76f2c-114">AES-256</span></span>|
|<span data-ttu-id="76f2c-115">des</span><span class="sxs-lookup"><span data-stu-id="76f2c-115">des</span></span>|<span data-ttu-id="76f2c-116">1</span><span class="sxs-lookup"><span data-stu-id="76f2c-116">1</span></span>|<span data-ttu-id="76f2c-117">DES</span><span class="sxs-lookup"><span data-stu-id="76f2c-117">DES</span></span>|
|<span data-ttu-id="76f2c-118">tripleDes</span><span class="sxs-lookup"><span data-stu-id="76f2c-118">tripleDes</span></span>|<span data-ttu-id="76f2c-119">双面</span><span class="sxs-lookup"><span data-stu-id="76f2c-119">2</span></span>|<span data-ttu-id="76f2c-120">3DES</span><span class="sxs-lookup"><span data-stu-id="76f2c-120">3DES</span></span>|
|<span data-ttu-id="76f2c-121">aes128-cts-hmac-sha1</span><span class="sxs-lookup"><span data-stu-id="76f2c-121">aes128</span></span>|<span data-ttu-id="76f2c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="76f2c-122">3</span></span>|<span data-ttu-id="76f2c-123">AES-128</span><span class="sxs-lookup"><span data-stu-id="76f2c-123">AES-128</span></span>|
|<span data-ttu-id="76f2c-124">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="76f2c-124">aes128Gcm</span></span>|<span data-ttu-id="76f2c-125">4 </span><span class="sxs-lookup"><span data-stu-id="76f2c-125">4</span></span>|<span data-ttu-id="76f2c-126">AES-128-GCM (16-八进制 ICV) </span><span class="sxs-lookup"><span data-stu-id="76f2c-126">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="76f2c-127">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="76f2c-127">aes256Gcm</span></span>|<span data-ttu-id="76f2c-128">5 </span><span class="sxs-lookup"><span data-stu-id="76f2c-128">5</span></span>|<span data-ttu-id="76f2c-129">AES-256-GCM (16-八进制 ICV) </span><span class="sxs-lookup"><span data-stu-id="76f2c-129">AES-256-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="76f2c-130">aes192</span><span class="sxs-lookup"><span data-stu-id="76f2c-130">aes192</span></span>|<span data-ttu-id="76f2c-131">6 </span><span class="sxs-lookup"><span data-stu-id="76f2c-131">6</span></span>|<span data-ttu-id="76f2c-132">AES-192</span><span class="sxs-lookup"><span data-stu-id="76f2c-132">AES-192</span></span>|
|<span data-ttu-id="76f2c-133">aes192Gcm</span><span class="sxs-lookup"><span data-stu-id="76f2c-133">aes192Gcm</span></span>|<span data-ttu-id="76f2c-134">7 </span><span class="sxs-lookup"><span data-stu-id="76f2c-134">7</span></span>|<span data-ttu-id="76f2c-135">AES-192-GCM</span><span class="sxs-lookup"><span data-stu-id="76f2c-135">AES-192-GCM</span></span>|




