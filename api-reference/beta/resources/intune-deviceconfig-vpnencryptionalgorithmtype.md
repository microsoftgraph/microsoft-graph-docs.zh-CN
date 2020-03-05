---
title: vpnEncryptionAlgorithmType 枚举类型
description: VPN 安全关联加密算法的类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f21a59e5be58f37ac69da1c12ceea17e64699a53
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529319"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="369db-103">vpnEncryptionAlgorithmType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="369db-103">vpnEncryptionAlgorithmType enum type</span></span>

<span data-ttu-id="369db-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="369db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="369db-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="369db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="369db-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="369db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="369db-107">VPN 安全关联加密算法的类型</span><span class="sxs-lookup"><span data-stu-id="369db-107">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="369db-108">成员</span><span class="sxs-lookup"><span data-stu-id="369db-108">Members</span></span>
|<span data-ttu-id="369db-109">成员</span><span class="sxs-lookup"><span data-stu-id="369db-109">Member</span></span>|<span data-ttu-id="369db-110">值</span><span class="sxs-lookup"><span data-stu-id="369db-110">Value</span></span>|<span data-ttu-id="369db-111">说明</span><span class="sxs-lookup"><span data-stu-id="369db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="369db-112">aes256</span><span class="sxs-lookup"><span data-stu-id="369db-112">aes256</span></span>|<span data-ttu-id="369db-113">0</span><span class="sxs-lookup"><span data-stu-id="369db-113">0</span></span>|<span data-ttu-id="369db-114">AES-256</span><span class="sxs-lookup"><span data-stu-id="369db-114">AES-256</span></span>|
|<span data-ttu-id="369db-115">des</span><span class="sxs-lookup"><span data-stu-id="369db-115">des</span></span>|<span data-ttu-id="369db-116">1 </span><span class="sxs-lookup"><span data-stu-id="369db-116">1</span></span>|<span data-ttu-id="369db-117">DES</span><span class="sxs-lookup"><span data-stu-id="369db-117">DES</span></span>|
|<span data-ttu-id="369db-118">tripleDes</span><span class="sxs-lookup"><span data-stu-id="369db-118">tripleDes</span></span>|<span data-ttu-id="369db-119">2 </span><span class="sxs-lookup"><span data-stu-id="369db-119">2</span></span>|<span data-ttu-id="369db-120">3DES</span><span class="sxs-lookup"><span data-stu-id="369db-120">3DES</span></span>|
|<span data-ttu-id="369db-121">aes128-cts-hmac-sha1</span><span class="sxs-lookup"><span data-stu-id="369db-121">aes128</span></span>|<span data-ttu-id="369db-122">3 </span><span class="sxs-lookup"><span data-stu-id="369db-122">3</span></span>|<span data-ttu-id="369db-123">AES-128</span><span class="sxs-lookup"><span data-stu-id="369db-123">AES-128</span></span>|
|<span data-ttu-id="369db-124">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="369db-124">aes128Gcm</span></span>|<span data-ttu-id="369db-125">4 </span><span class="sxs-lookup"><span data-stu-id="369db-125">4</span></span>|<span data-ttu-id="369db-126">AES-128-GCM （16-八进制的 ICV）</span><span class="sxs-lookup"><span data-stu-id="369db-126">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="369db-127">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="369db-127">aes256Gcm</span></span>|<span data-ttu-id="369db-128">5 </span><span class="sxs-lookup"><span data-stu-id="369db-128">5</span></span>|<span data-ttu-id="369db-129">AES-256-GCM （16-八进制的 ICV）</span><span class="sxs-lookup"><span data-stu-id="369db-129">AES-256-GCM (16-octet ICV)</span></span>|



