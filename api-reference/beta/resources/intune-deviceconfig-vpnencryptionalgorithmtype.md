---
title: vpnEncryptionAlgorithmType 枚举类型
description: VPN 安全关联加密算法的类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 30cf31343a18f0558494b5d660d9197e6606a223
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367713"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="cfda0-103">vpnEncryptionAlgorithmType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cfda0-103">vpnEncryptionAlgorithmType enum type</span></span>

> <span data-ttu-id="cfda0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cfda0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfda0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cfda0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfda0-106">VPN 安全关联加密算法的类型</span><span class="sxs-lookup"><span data-stu-id="cfda0-106">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="cfda0-107">成员</span><span class="sxs-lookup"><span data-stu-id="cfda0-107">Members</span></span>
|<span data-ttu-id="cfda0-108">成员</span><span class="sxs-lookup"><span data-stu-id="cfda0-108">Member</span></span>|<span data-ttu-id="cfda0-109">值</span><span class="sxs-lookup"><span data-stu-id="cfda0-109">Value</span></span>|<span data-ttu-id="cfda0-110">说明</span><span class="sxs-lookup"><span data-stu-id="cfda0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfda0-111">aes256</span><span class="sxs-lookup"><span data-stu-id="cfda0-111">aes256</span></span>|<span data-ttu-id="cfda0-112">0</span><span class="sxs-lookup"><span data-stu-id="cfda0-112">0</span></span>|<span data-ttu-id="cfda0-113">AES-256</span><span class="sxs-lookup"><span data-stu-id="cfda0-113">AES-256</span></span>|
|<span data-ttu-id="cfda0-114">des</span><span class="sxs-lookup"><span data-stu-id="cfda0-114">des</span></span>|<span data-ttu-id="cfda0-115">1</span><span class="sxs-lookup"><span data-stu-id="cfda0-115">1</span></span>|<span data-ttu-id="cfda0-116">DES</span><span class="sxs-lookup"><span data-stu-id="cfda0-116">DES</span></span>|
|<span data-ttu-id="cfda0-117">tripleDes</span><span class="sxs-lookup"><span data-stu-id="cfda0-117">tripleDes</span></span>|<span data-ttu-id="cfda0-118">双面</span><span class="sxs-lookup"><span data-stu-id="cfda0-118">2</span></span>|<span data-ttu-id="cfda0-119">3DES</span><span class="sxs-lookup"><span data-stu-id="cfda0-119">3DES</span></span>|
|<span data-ttu-id="cfda0-120">aes128-cts-hmac-sha1</span><span class="sxs-lookup"><span data-stu-id="cfda0-120">aes128</span></span>|<span data-ttu-id="cfda0-121">第三章</span><span class="sxs-lookup"><span data-stu-id="cfda0-121">3</span></span>|<span data-ttu-id="cfda0-122">AES-128</span><span class="sxs-lookup"><span data-stu-id="cfda0-122">AES-128</span></span>|
|<span data-ttu-id="cfda0-123">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="cfda0-123">aes128Gcm</span></span>|<span data-ttu-id="cfda0-124">4</span><span class="sxs-lookup"><span data-stu-id="cfda0-124">4</span></span>|<span data-ttu-id="cfda0-125">AES-128-GCM (16-八进制的 ICV)</span><span class="sxs-lookup"><span data-stu-id="cfda0-125">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="cfda0-126">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="cfda0-126">aes256Gcm</span></span>|<span data-ttu-id="cfda0-127">5</span><span class="sxs-lookup"><span data-stu-id="cfda0-127">5</span></span>|<span data-ttu-id="cfda0-128">AES-256-GCM (16-八进制的 ICV)</span><span class="sxs-lookup"><span data-stu-id="cfda0-128">AES-256-GCM (16-octet ICV)</span></span>|



