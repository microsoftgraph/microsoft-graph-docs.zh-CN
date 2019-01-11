---
title: fileHashType 枚举
description: 文件哈希类型的枚举。
localization_priority: Normal
ms.openlocfilehash: e1c31aaea6c8cea40817efea61dc8654d3d17fae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816328"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="00ba0-103">fileHashType 枚举</span><span class="sxs-lookup"><span data-stu-id="00ba0-103">fileHashType enum</span></span>

> <span data-ttu-id="00ba0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="00ba0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00ba0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00ba0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00ba0-106">文件哈希类型的枚举。</span><span class="sxs-lookup"><span data-stu-id="00ba0-106">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="00ba0-107">成员</span><span class="sxs-lookup"><span data-stu-id="00ba0-107">Members</span></span>

|<span data-ttu-id="00ba0-108">成员</span><span class="sxs-lookup"><span data-stu-id="00ba0-108">Member</span></span>|<span data-ttu-id="00ba0-109">值</span><span class="sxs-lookup"><span data-stu-id="00ba0-109">Value</span></span>|<span data-ttu-id="00ba0-110">Description</span><span class="sxs-lookup"><span data-stu-id="00ba0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00ba0-111">unknown</span><span class="sxs-lookup"><span data-stu-id="00ba0-111">unknown</span></span>|<span data-ttu-id="00ba0-112">0</span><span class="sxs-lookup"><span data-stu-id="00ba0-112">0</span></span>|<span data-ttu-id="00ba0-113">未知的类型。</span><span class="sxs-lookup"><span data-stu-id="00ba0-113">Unknown type.</span></span>|
|<span data-ttu-id="00ba0-114">sha1</span><span class="sxs-lookup"><span data-stu-id="00ba0-114">sha1</span></span>|<span data-ttu-id="00ba0-115">1</span><span class="sxs-lookup"><span data-stu-id="00ba0-115">1</span></span>|<span data-ttu-id="00ba0-116">SHA1 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="00ba0-116">SHA1 hash type.</span></span>|
|<span data-ttu-id="00ba0-117">sha256</span><span class="sxs-lookup"><span data-stu-id="00ba0-117">sha256</span></span>|<span data-ttu-id="00ba0-118">2</span><span class="sxs-lookup"><span data-stu-id="00ba0-118">2</span></span>| <span data-ttu-id="00ba0-119">SHA256 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="00ba0-119">SHA256 hash type.</span></span>|
|<span data-ttu-id="00ba0-120">md5</span><span class="sxs-lookup"><span data-stu-id="00ba0-120">md5</span></span>|<span data-ttu-id="00ba0-121">3</span><span class="sxs-lookup"><span data-stu-id="00ba0-121">3</span></span>| <span data-ttu-id="00ba0-122">MD5 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="00ba0-122">MD5 hash type.</span></span>|
|<span data-ttu-id="00ba0-123">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="00ba0-123">authenticodeHash256</span></span>|<span data-ttu-id="00ba0-124">4</span><span class="sxs-lookup"><span data-stu-id="00ba0-124">4</span></span>| <span data-ttu-id="00ba0-125">AuthenticodeHash256 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="00ba0-125">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="00ba0-126">lsHash</span><span class="sxs-lookup"><span data-stu-id="00ba0-126">lsHash</span></span>|<span data-ttu-id="00ba0-127">5</span><span class="sxs-lookup"><span data-stu-id="00ba0-127">5</span></span>| <span data-ttu-id="00ba0-128">LsHash 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="00ba0-128">LsHash hash type.</span></span>|
|<span data-ttu-id="00ba0-129">ctph</span><span class="sxs-lookup"><span data-stu-id="00ba0-129">ctph</span></span>|<span data-ttu-id="00ba0-130">6</span><span class="sxs-lookup"><span data-stu-id="00ba0-130">6</span></span>| <span data-ttu-id="00ba0-131">CTPH 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="00ba0-131">CTPH hash type.</span></span>|
|<span data-ttu-id="00ba0-132">peSha1</span><span class="sxs-lookup"><span data-stu-id="00ba0-132">peSha1</span></span>|<span data-ttu-id="00ba0-133">7</span><span class="sxs-lookup"><span data-stu-id="00ba0-133">7</span></span>| <span data-ttu-id="00ba0-134">PESHA1 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="00ba0-134">PESHA1 hash type.</span></span>|
|<span data-ttu-id="00ba0-135">peSha256</span><span class="sxs-lookup"><span data-stu-id="00ba0-135">peSha256</span></span>|<span data-ttu-id="00ba0-136">8</span><span class="sxs-lookup"><span data-stu-id="00ba0-136">8</span></span>| <span data-ttu-id="00ba0-137">PESHA256 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="00ba0-137">PESHA256 hash type.</span></span>|
