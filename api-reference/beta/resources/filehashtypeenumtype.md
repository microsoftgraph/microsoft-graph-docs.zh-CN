---
title: fileHashType 枚举
description: 文件哈希类型的枚举。
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c0d8c87f79580107d56ec84aa9b1a4bc397d4171
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154141"
---
# <a name="filehashtype-enum-type"></a><span data-ttu-id="8a6da-103">fileHashType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8a6da-103">fileHashType enum type</span></span>

<span data-ttu-id="8a6da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a6da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a6da-105">文件哈希类型的枚举。</span><span class="sxs-lookup"><span data-stu-id="8a6da-105">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="8a6da-106">成员</span><span class="sxs-lookup"><span data-stu-id="8a6da-106">Members</span></span>

|<span data-ttu-id="8a6da-107">成员</span><span class="sxs-lookup"><span data-stu-id="8a6da-107">Member</span></span>|<span data-ttu-id="8a6da-108">值</span><span class="sxs-lookup"><span data-stu-id="8a6da-108">Value</span></span>|<span data-ttu-id="8a6da-109">Description</span><span class="sxs-lookup"><span data-stu-id="8a6da-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a6da-110">unknown</span><span class="sxs-lookup"><span data-stu-id="8a6da-110">unknown</span></span>|<span data-ttu-id="8a6da-111">0</span><span class="sxs-lookup"><span data-stu-id="8a6da-111">0</span></span>|<span data-ttu-id="8a6da-112">未知类型。</span><span class="sxs-lookup"><span data-stu-id="8a6da-112">Unknown type.</span></span>|
|<span data-ttu-id="8a6da-113">sha1</span><span class="sxs-lookup"><span data-stu-id="8a6da-113">sha1</span></span>|<span data-ttu-id="8a6da-114">1</span><span class="sxs-lookup"><span data-stu-id="8a6da-114">1</span></span>|<span data-ttu-id="8a6da-115">SHA1 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="8a6da-115">SHA1 hash type.</span></span>|
|<span data-ttu-id="8a6da-116">sha256</span><span class="sxs-lookup"><span data-stu-id="8a6da-116">sha256</span></span>|<span data-ttu-id="8a6da-117">双面</span><span class="sxs-lookup"><span data-stu-id="8a6da-117">2</span></span>| <span data-ttu-id="8a6da-118">SHA256 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="8a6da-118">SHA256 hash type.</span></span>|
|<span data-ttu-id="8a6da-119">md5</span><span class="sxs-lookup"><span data-stu-id="8a6da-119">md5</span></span>|<span data-ttu-id="8a6da-120">第三章</span><span class="sxs-lookup"><span data-stu-id="8a6da-120">3</span></span>| <span data-ttu-id="8a6da-121">MD5 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="8a6da-121">MD5 hash type.</span></span>|
|<span data-ttu-id="8a6da-122">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="8a6da-122">authenticodeHash256</span></span>|<span data-ttu-id="8a6da-123">4 </span><span class="sxs-lookup"><span data-stu-id="8a6da-123">4</span></span>| <span data-ttu-id="8a6da-124">AuthenticodeHash256 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="8a6da-124">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="8a6da-125">lsHash</span><span class="sxs-lookup"><span data-stu-id="8a6da-125">lsHash</span></span>|<span data-ttu-id="8a6da-126">5 </span><span class="sxs-lookup"><span data-stu-id="8a6da-126">5</span></span>| <span data-ttu-id="8a6da-127">LsHash 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="8a6da-127">LsHash hash type.</span></span>|
|<span data-ttu-id="8a6da-128">ctph</span><span class="sxs-lookup"><span data-stu-id="8a6da-128">ctph</span></span>|<span data-ttu-id="8a6da-129">6 </span><span class="sxs-lookup"><span data-stu-id="8a6da-129">6</span></span>| <span data-ttu-id="8a6da-130">CTPH 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="8a6da-130">CTPH hash type.</span></span>|
|<span data-ttu-id="8a6da-131">peSha1</span><span class="sxs-lookup"><span data-stu-id="8a6da-131">peSha1</span></span>|<span data-ttu-id="8a6da-132">7 </span><span class="sxs-lookup"><span data-stu-id="8a6da-132">7</span></span>| <span data-ttu-id="8a6da-133">PESHA1 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="8a6da-133">PESHA1 hash type.</span></span>|
|<span data-ttu-id="8a6da-134">peSha256</span><span class="sxs-lookup"><span data-stu-id="8a6da-134">peSha256</span></span>|<span data-ttu-id="8a6da-135">8 </span><span class="sxs-lookup"><span data-stu-id="8a6da-135">8</span></span>| <span data-ttu-id="8a6da-136">PESHA256 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="8a6da-136">PESHA256 hash type.</span></span>|
