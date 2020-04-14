---
title: vpnEncryptionAlgorithmType 枚举类型
description: VPN 安全关联加密算法的类型
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: df8b0d5baaf0dd947af97a87e370aa76814d6fef
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412206"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="42a5d-103">vpnEncryptionAlgorithmType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="42a5d-103">vpnEncryptionAlgorithmType enum type</span></span>

<span data-ttu-id="42a5d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42a5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42a5d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42a5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42a5d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42a5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42a5d-107">VPN 安全关联加密算法的类型</span><span class="sxs-lookup"><span data-stu-id="42a5d-107">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="42a5d-108">成员</span><span class="sxs-lookup"><span data-stu-id="42a5d-108">Members</span></span>
|<span data-ttu-id="42a5d-109">成员</span><span class="sxs-lookup"><span data-stu-id="42a5d-109">Member</span></span>|<span data-ttu-id="42a5d-110">值</span><span class="sxs-lookup"><span data-stu-id="42a5d-110">Value</span></span>|<span data-ttu-id="42a5d-111">说明</span><span class="sxs-lookup"><span data-stu-id="42a5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42a5d-112">aes256</span><span class="sxs-lookup"><span data-stu-id="42a5d-112">aes256</span></span>|<span data-ttu-id="42a5d-113">0</span><span class="sxs-lookup"><span data-stu-id="42a5d-113">0</span></span>|<span data-ttu-id="42a5d-114">AES-256</span><span class="sxs-lookup"><span data-stu-id="42a5d-114">AES-256</span></span>|
|<span data-ttu-id="42a5d-115">des</span><span class="sxs-lookup"><span data-stu-id="42a5d-115">des</span></span>|<span data-ttu-id="42a5d-116">1</span><span class="sxs-lookup"><span data-stu-id="42a5d-116">1</span></span>|<span data-ttu-id="42a5d-117">DES</span><span class="sxs-lookup"><span data-stu-id="42a5d-117">DES</span></span>|
|<span data-ttu-id="42a5d-118">tripleDes</span><span class="sxs-lookup"><span data-stu-id="42a5d-118">tripleDes</span></span>|<span data-ttu-id="42a5d-119">双面</span><span class="sxs-lookup"><span data-stu-id="42a5d-119">2</span></span>|<span data-ttu-id="42a5d-120">3DES</span><span class="sxs-lookup"><span data-stu-id="42a5d-120">3DES</span></span>|
|<span data-ttu-id="42a5d-121">aes128-cts-hmac-sha1</span><span class="sxs-lookup"><span data-stu-id="42a5d-121">aes128</span></span>|<span data-ttu-id="42a5d-122">第三章</span><span class="sxs-lookup"><span data-stu-id="42a5d-122">3</span></span>|<span data-ttu-id="42a5d-123">AES-128</span><span class="sxs-lookup"><span data-stu-id="42a5d-123">AES-128</span></span>|
|<span data-ttu-id="42a5d-124">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="42a5d-124">aes128Gcm</span></span>|<span data-ttu-id="42a5d-125">4 </span><span class="sxs-lookup"><span data-stu-id="42a5d-125">4</span></span>|<span data-ttu-id="42a5d-126">AES-128-GCM （16-八进制的 ICV）</span><span class="sxs-lookup"><span data-stu-id="42a5d-126">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="42a5d-127">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="42a5d-127">aes256Gcm</span></span>|<span data-ttu-id="42a5d-128">5 </span><span class="sxs-lookup"><span data-stu-id="42a5d-128">5</span></span>|<span data-ttu-id="42a5d-129">AES-256-GCM （16-八进制的 ICV）</span><span class="sxs-lookup"><span data-stu-id="42a5d-129">AES-256-GCM (16-octet ICV)</span></span>|



