---
title: userPfxPaddingScheme 枚举类型
description: 加密提供程序使用的填充方案的受支持的值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6b04dcd01d21ace78368411524067f83db3bc93a
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163547"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="3465c-103">userPfxPaddingScheme 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3465c-103">userPfxPaddingScheme enum type</span></span>

> <span data-ttu-id="3465c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3465c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3465c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3465c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3465c-106">加密提供程序使用的填充方案的受支持的值。</span><span class="sxs-lookup"><span data-stu-id="3465c-106">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="3465c-107">成员</span><span class="sxs-lookup"><span data-stu-id="3465c-107">Members</span></span>
|<span data-ttu-id="3465c-108">成员</span><span class="sxs-lookup"><span data-stu-id="3465c-108">Member</span></span>|<span data-ttu-id="3465c-109">值</span><span class="sxs-lookup"><span data-stu-id="3465c-109">Value</span></span>|<span data-ttu-id="3465c-110">说明</span><span class="sxs-lookup"><span data-stu-id="3465c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3465c-111">无</span><span class="sxs-lookup"><span data-stu-id="3465c-111">none</span></span>|<span data-ttu-id="3465c-112">0</span><span class="sxs-lookup"><span data-stu-id="3465c-112">0</span></span>|<span data-ttu-id="3465c-113">未知的填充方案。</span><span class="sxs-lookup"><span data-stu-id="3465c-113">Unknown padding Scheme.</span></span>|
|<span data-ttu-id="3465c-114">pkcs1</span><span class="sxs-lookup"><span data-stu-id="3465c-114">pkcs1</span></span>|<span data-ttu-id="3465c-115">1</span><span class="sxs-lookup"><span data-stu-id="3465c-115">1</span></span>|<span data-ttu-id="3465c-116">不再支持 Pkcs1</span><span class="sxs-lookup"><span data-stu-id="3465c-116">Pkcs1 is no longer supported</span></span>|
|<span data-ttu-id="3465c-117">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="3465c-117">oaepSha1</span></span>|<span data-ttu-id="3465c-118">双面</span><span class="sxs-lookup"><span data-stu-id="3465c-118">2</span></span>|<span data-ttu-id="3465c-119">不再支持 OaepSha1</span><span class="sxs-lookup"><span data-stu-id="3465c-119">OaepSha1 is no longer supported</span></span>|
|<span data-ttu-id="3465c-120">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="3465c-120">oaepSha256</span></span>|<span data-ttu-id="3465c-121">第三章</span><span class="sxs-lookup"><span data-stu-id="3465c-121">3</span></span>|<span data-ttu-id="3465c-122">使用 OAEP SHA-256 填充。</span><span class="sxs-lookup"><span data-stu-id="3465c-122">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="3465c-123">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="3465c-123">oaepSha384</span></span>|<span data-ttu-id="3465c-124">4</span><span class="sxs-lookup"><span data-stu-id="3465c-124">4</span></span>|<span data-ttu-id="3465c-125">使用 OAEP SHA-384 填充。</span><span class="sxs-lookup"><span data-stu-id="3465c-125">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="3465c-126">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="3465c-126">oaepSha512</span></span>|<span data-ttu-id="3465c-127">5</span><span class="sxs-lookup"><span data-stu-id="3465c-127">5</span></span>|<span data-ttu-id="3465c-128">使用 OAEP SHA-512 填充。</span><span class="sxs-lookup"><span data-stu-id="3465c-128">Use OAEP SHA-512 padding.</span></span>|



