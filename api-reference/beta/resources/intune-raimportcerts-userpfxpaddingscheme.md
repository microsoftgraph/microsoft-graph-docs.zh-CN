---
title: userPfxPaddingScheme 枚举类型
description: 加密提供程序使用的填充方案的受支持的值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0cbdc056c1dc0ea1aa73ae0cd96af428ce9f2bf3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307168"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="551bb-103">userPfxPaddingScheme 枚举类型</span><span class="sxs-lookup"><span data-stu-id="551bb-103">userPfxPaddingScheme enum type</span></span>

<span data-ttu-id="551bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="551bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="551bb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="551bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="551bb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="551bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="551bb-107">加密提供程序使用的填充方案的受支持的值。</span><span class="sxs-lookup"><span data-stu-id="551bb-107">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="551bb-108">成员</span><span class="sxs-lookup"><span data-stu-id="551bb-108">Members</span></span>
|<span data-ttu-id="551bb-109">成员</span><span class="sxs-lookup"><span data-stu-id="551bb-109">Member</span></span>|<span data-ttu-id="551bb-110">值</span><span class="sxs-lookup"><span data-stu-id="551bb-110">Value</span></span>|<span data-ttu-id="551bb-111">Description</span><span class="sxs-lookup"><span data-stu-id="551bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="551bb-112">无</span><span class="sxs-lookup"><span data-stu-id="551bb-112">none</span></span>|<span data-ttu-id="551bb-113">0</span><span class="sxs-lookup"><span data-stu-id="551bb-113">0</span></span>|<span data-ttu-id="551bb-114">未知的填充方案。</span><span class="sxs-lookup"><span data-stu-id="551bb-114">Unknown padding Scheme.</span></span>|
|<span data-ttu-id="551bb-115">pkcs1</span><span class="sxs-lookup"><span data-stu-id="551bb-115">pkcs1</span></span>|<span data-ttu-id="551bb-116">1</span><span class="sxs-lookup"><span data-stu-id="551bb-116">1</span></span>|<span data-ttu-id="551bb-117">不再支持 Pkcs1</span><span class="sxs-lookup"><span data-stu-id="551bb-117">Pkcs1 is no longer supported</span></span>|
|<span data-ttu-id="551bb-118">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="551bb-118">oaepSha1</span></span>|<span data-ttu-id="551bb-119">双面</span><span class="sxs-lookup"><span data-stu-id="551bb-119">2</span></span>|<span data-ttu-id="551bb-120">不再支持 OaepSha1</span><span class="sxs-lookup"><span data-stu-id="551bb-120">OaepSha1 is no longer supported</span></span>|
|<span data-ttu-id="551bb-121">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="551bb-121">oaepSha256</span></span>|<span data-ttu-id="551bb-122">第三章</span><span class="sxs-lookup"><span data-stu-id="551bb-122">3</span></span>|<span data-ttu-id="551bb-123">使用 OAEP SHA-256 填充。</span><span class="sxs-lookup"><span data-stu-id="551bb-123">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="551bb-124">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="551bb-124">oaepSha384</span></span>|<span data-ttu-id="551bb-125">4 </span><span class="sxs-lookup"><span data-stu-id="551bb-125">4</span></span>|<span data-ttu-id="551bb-126">使用 OAEP SHA-384 填充。</span><span class="sxs-lookup"><span data-stu-id="551bb-126">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="551bb-127">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="551bb-127">oaepSha512</span></span>|<span data-ttu-id="551bb-128">5 </span><span class="sxs-lookup"><span data-stu-id="551bb-128">5</span></span>|<span data-ttu-id="551bb-129">使用 OAEP SHA-512 填充。</span><span class="sxs-lookup"><span data-stu-id="551bb-129">Use OAEP SHA-512 padding.</span></span>|




