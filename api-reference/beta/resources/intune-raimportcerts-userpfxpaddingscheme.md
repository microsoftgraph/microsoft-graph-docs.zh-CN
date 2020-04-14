---
title: userPfxPaddingScheme 枚举类型
description: 加密提供程序使用的填充方案的受支持的值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3e96dc40ca742c802a1b2bc88e05a708202648bc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467716"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="1aee9-103">userPfxPaddingScheme 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1aee9-103">userPfxPaddingScheme enum type</span></span>

<span data-ttu-id="1aee9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1aee9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1aee9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1aee9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1aee9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1aee9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aee9-107">加密提供程序使用的填充方案的受支持的值。</span><span class="sxs-lookup"><span data-stu-id="1aee9-107">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="1aee9-108">成员</span><span class="sxs-lookup"><span data-stu-id="1aee9-108">Members</span></span>
|<span data-ttu-id="1aee9-109">成员</span><span class="sxs-lookup"><span data-stu-id="1aee9-109">Member</span></span>|<span data-ttu-id="1aee9-110">值</span><span class="sxs-lookup"><span data-stu-id="1aee9-110">Value</span></span>|<span data-ttu-id="1aee9-111">说明</span><span class="sxs-lookup"><span data-stu-id="1aee9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aee9-112">无</span><span class="sxs-lookup"><span data-stu-id="1aee9-112">none</span></span>|<span data-ttu-id="1aee9-113">0</span><span class="sxs-lookup"><span data-stu-id="1aee9-113">0</span></span>|<span data-ttu-id="1aee9-114">未知的填充方案。</span><span class="sxs-lookup"><span data-stu-id="1aee9-114">Unknown padding Scheme.</span></span>|
|<span data-ttu-id="1aee9-115">pkcs1</span><span class="sxs-lookup"><span data-stu-id="1aee9-115">pkcs1</span></span>|<span data-ttu-id="1aee9-116">1</span><span class="sxs-lookup"><span data-stu-id="1aee9-116">1</span></span>|<span data-ttu-id="1aee9-117">不再支持 Pkcs1</span><span class="sxs-lookup"><span data-stu-id="1aee9-117">Pkcs1 is no longer supported</span></span>|
|<span data-ttu-id="1aee9-118">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="1aee9-118">oaepSha1</span></span>|<span data-ttu-id="1aee9-119">双面</span><span class="sxs-lookup"><span data-stu-id="1aee9-119">2</span></span>|<span data-ttu-id="1aee9-120">不再支持 OaepSha1</span><span class="sxs-lookup"><span data-stu-id="1aee9-120">OaepSha1 is no longer supported</span></span>|
|<span data-ttu-id="1aee9-121">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="1aee9-121">oaepSha256</span></span>|<span data-ttu-id="1aee9-122">第三章</span><span class="sxs-lookup"><span data-stu-id="1aee9-122">3</span></span>|<span data-ttu-id="1aee9-123">使用 OAEP SHA-256 填充。</span><span class="sxs-lookup"><span data-stu-id="1aee9-123">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="1aee9-124">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="1aee9-124">oaepSha384</span></span>|<span data-ttu-id="1aee9-125">4 </span><span class="sxs-lookup"><span data-stu-id="1aee9-125">4</span></span>|<span data-ttu-id="1aee9-126">使用 OAEP SHA-384 填充。</span><span class="sxs-lookup"><span data-stu-id="1aee9-126">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="1aee9-127">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="1aee9-127">oaepSha512</span></span>|<span data-ttu-id="1aee9-128">5 </span><span class="sxs-lookup"><span data-stu-id="1aee9-128">5</span></span>|<span data-ttu-id="1aee9-129">使用 OAEP SHA-512 填充。</span><span class="sxs-lookup"><span data-stu-id="1aee9-129">Use OAEP SHA-512 padding.</span></span>|



