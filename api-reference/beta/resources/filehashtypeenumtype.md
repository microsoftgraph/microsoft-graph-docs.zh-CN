---
title: fileHashType 枚举
description: 文件哈希类型的枚举。
ms.openlocfilehash: fbaa390ee8c543d2ed7c77cc05a11b519df0da9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042171"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="abcfb-103">fileHashType 枚举</span><span class="sxs-lookup"><span data-stu-id="abcfb-103">fileHashType enum</span></span>

> <span data-ttu-id="abcfb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="abcfb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abcfb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="abcfb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="abcfb-106">文件哈希类型的枚举。</span><span class="sxs-lookup"><span data-stu-id="abcfb-106">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="abcfb-107">成员</span><span class="sxs-lookup"><span data-stu-id="abcfb-107">Members</span></span>

|<span data-ttu-id="abcfb-108">成员</span><span class="sxs-lookup"><span data-stu-id="abcfb-108">Member</span></span>|<span data-ttu-id="abcfb-109">值</span><span class="sxs-lookup"><span data-stu-id="abcfb-109">Value</span></span>|<span data-ttu-id="abcfb-110">说明</span><span class="sxs-lookup"><span data-stu-id="abcfb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abcfb-111">unknown</span><span class="sxs-lookup"><span data-stu-id="abcfb-111">unknown</span></span>|<span data-ttu-id="abcfb-112">0</span><span class="sxs-lookup"><span data-stu-id="abcfb-112">0</span></span>|<span data-ttu-id="abcfb-113">未知的类型。</span><span class="sxs-lookup"><span data-stu-id="abcfb-113">Unknown type.</span></span>|
|<span data-ttu-id="abcfb-114">sha1</span><span class="sxs-lookup"><span data-stu-id="abcfb-114">sha1</span></span>|<span data-ttu-id="abcfb-115">1</span><span class="sxs-lookup"><span data-stu-id="abcfb-115">1</span></span>|<span data-ttu-id="abcfb-116">SHA1 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="abcfb-116">SHA1 hash type.</span></span>|
|<span data-ttu-id="abcfb-117">sha256</span><span class="sxs-lookup"><span data-stu-id="abcfb-117">sha256</span></span>|<span data-ttu-id="abcfb-118">2</span><span class="sxs-lookup"><span data-stu-id="abcfb-118">2</span></span>| <span data-ttu-id="abcfb-119">SHA256 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="abcfb-119">SHA256 hash type.</span></span>|
|<span data-ttu-id="abcfb-120">md5</span><span class="sxs-lookup"><span data-stu-id="abcfb-120">md5</span></span>|<span data-ttu-id="abcfb-121">3</span><span class="sxs-lookup"><span data-stu-id="abcfb-121">3</span></span>| <span data-ttu-id="abcfb-122">MD5 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="abcfb-122">MD5 hash type.</span></span>|
|<span data-ttu-id="abcfb-123">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="abcfb-123">authenticodeHash256</span></span>|<span data-ttu-id="abcfb-124">4</span><span class="sxs-lookup"><span data-stu-id="abcfb-124">4</span></span>| <span data-ttu-id="abcfb-125">AuthenticodeHash256 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="abcfb-125">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="abcfb-126">lsHash</span><span class="sxs-lookup"><span data-stu-id="abcfb-126">lsHash</span></span>|<span data-ttu-id="abcfb-127">5</span><span class="sxs-lookup"><span data-stu-id="abcfb-127">5</span></span>| <span data-ttu-id="abcfb-128">LsHash 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="abcfb-128">LsHash hash type.</span></span>|
|<span data-ttu-id="abcfb-129">ctph</span><span class="sxs-lookup"><span data-stu-id="abcfb-129">ctph</span></span>|<span data-ttu-id="abcfb-130">6</span><span class="sxs-lookup"><span data-stu-id="abcfb-130">6</span></span>| <span data-ttu-id="abcfb-131">CTPH 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="abcfb-131">CTPH hash type.</span></span>|
|<span data-ttu-id="abcfb-132">peSha1</span><span class="sxs-lookup"><span data-stu-id="abcfb-132">peSha1</span></span>|<span data-ttu-id="abcfb-133">7</span><span class="sxs-lookup"><span data-stu-id="abcfb-133">7</span></span>| <span data-ttu-id="abcfb-134">PESHA1 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="abcfb-134">PESHA1 hash type.</span></span>|
|<span data-ttu-id="abcfb-135">peSha256</span><span class="sxs-lookup"><span data-stu-id="abcfb-135">peSha256</span></span>|<span data-ttu-id="abcfb-136">8</span><span class="sxs-lookup"><span data-stu-id="abcfb-136">8</span></span>| <span data-ttu-id="abcfb-137">PESHA256 哈希值类型。</span><span class="sxs-lookup"><span data-stu-id="abcfb-137">PESHA256 hash type.</span></span>|
