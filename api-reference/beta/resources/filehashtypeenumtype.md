---
title: fileHashType 枚举
description: 文件哈希类型的枚举。
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c8f2b733363ecbd79a885a0b76c170f076664590
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498215"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="c706e-103">fileHashType 枚举</span><span class="sxs-lookup"><span data-stu-id="c706e-103">fileHashType enum</span></span>

<span data-ttu-id="c706e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c706e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c706e-105">文件哈希类型的枚举。</span><span class="sxs-lookup"><span data-stu-id="c706e-105">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="c706e-106">成员</span><span class="sxs-lookup"><span data-stu-id="c706e-106">Members</span></span>

|<span data-ttu-id="c706e-107">成员</span><span class="sxs-lookup"><span data-stu-id="c706e-107">Member</span></span>|<span data-ttu-id="c706e-108">值</span><span class="sxs-lookup"><span data-stu-id="c706e-108">Value</span></span>|<span data-ttu-id="c706e-109">说明</span><span class="sxs-lookup"><span data-stu-id="c706e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c706e-110">unknown</span><span class="sxs-lookup"><span data-stu-id="c706e-110">unknown</span></span>|<span data-ttu-id="c706e-111">0</span><span class="sxs-lookup"><span data-stu-id="c706e-111">0</span></span>|<span data-ttu-id="c706e-112">未知类型。</span><span class="sxs-lookup"><span data-stu-id="c706e-112">Unknown type.</span></span>|
|<span data-ttu-id="c706e-113">sha1</span><span class="sxs-lookup"><span data-stu-id="c706e-113">sha1</span></span>|<span data-ttu-id="c706e-114">1 </span><span class="sxs-lookup"><span data-stu-id="c706e-114">1</span></span>|<span data-ttu-id="c706e-115">SHA1 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="c706e-115">SHA1 hash type.</span></span>|
|<span data-ttu-id="c706e-116">sha256</span><span class="sxs-lookup"><span data-stu-id="c706e-116">sha256</span></span>|<span data-ttu-id="c706e-117">2 </span><span class="sxs-lookup"><span data-stu-id="c706e-117">2</span></span>| <span data-ttu-id="c706e-118">SHA256 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="c706e-118">SHA256 hash type.</span></span>|
|<span data-ttu-id="c706e-119">md5</span><span class="sxs-lookup"><span data-stu-id="c706e-119">md5</span></span>|<span data-ttu-id="c706e-120">3 </span><span class="sxs-lookup"><span data-stu-id="c706e-120">3</span></span>| <span data-ttu-id="c706e-121">MD5 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="c706e-121">MD5 hash type.</span></span>|
|<span data-ttu-id="c706e-122">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="c706e-122">authenticodeHash256</span></span>|<span data-ttu-id="c706e-123">4 </span><span class="sxs-lookup"><span data-stu-id="c706e-123">4</span></span>| <span data-ttu-id="c706e-124">AuthenticodeHash256 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="c706e-124">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="c706e-125">lsHash</span><span class="sxs-lookup"><span data-stu-id="c706e-125">lsHash</span></span>|<span data-ttu-id="c706e-126">5 </span><span class="sxs-lookup"><span data-stu-id="c706e-126">5</span></span>| <span data-ttu-id="c706e-127">LsHash 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="c706e-127">LsHash hash type.</span></span>|
|<span data-ttu-id="c706e-128">ctph</span><span class="sxs-lookup"><span data-stu-id="c706e-128">ctph</span></span>|<span data-ttu-id="c706e-129">6 </span><span class="sxs-lookup"><span data-stu-id="c706e-129">6</span></span>| <span data-ttu-id="c706e-130">CTPH 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="c706e-130">CTPH hash type.</span></span>|
|<span data-ttu-id="c706e-131">peSha1</span><span class="sxs-lookup"><span data-stu-id="c706e-131">peSha1</span></span>|<span data-ttu-id="c706e-132">7 </span><span class="sxs-lookup"><span data-stu-id="c706e-132">7</span></span>| <span data-ttu-id="c706e-133">PESHA1 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="c706e-133">PESHA1 hash type.</span></span>|
|<span data-ttu-id="c706e-134">peSha256</span><span class="sxs-lookup"><span data-stu-id="c706e-134">peSha256</span></span>|<span data-ttu-id="c706e-135">8 </span><span class="sxs-lookup"><span data-stu-id="c706e-135">8</span></span>| <span data-ttu-id="c706e-136">PESHA256 哈希类型。</span><span class="sxs-lookup"><span data-stu-id="c706e-136">PESHA256 hash type.</span></span>|
