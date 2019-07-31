---
title: userPfxPaddingScheme 枚举类型
description: 加密提供程序使用的填充方案的受支持的值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a3c4d4d07a3891167838af6de7ea854883a5b1e5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967698"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="b97b6-103">userPfxPaddingScheme 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b97b6-103">userPfxPaddingScheme enum type</span></span>

> <span data-ttu-id="b97b6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b97b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b97b6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b97b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b97b6-106">加密提供程序使用的填充方案的受支持的值。</span><span class="sxs-lookup"><span data-stu-id="b97b6-106">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="b97b6-107">成员</span><span class="sxs-lookup"><span data-stu-id="b97b6-107">Members</span></span>
|<span data-ttu-id="b97b6-108">成员</span><span class="sxs-lookup"><span data-stu-id="b97b6-108">Member</span></span>|<span data-ttu-id="b97b6-109">值</span><span class="sxs-lookup"><span data-stu-id="b97b6-109">Value</span></span>|<span data-ttu-id="b97b6-110">说明</span><span class="sxs-lookup"><span data-stu-id="b97b6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b97b6-111">无</span><span class="sxs-lookup"><span data-stu-id="b97b6-111">none</span></span>|<span data-ttu-id="b97b6-112">0</span><span class="sxs-lookup"><span data-stu-id="b97b6-112">0</span></span>|<span data-ttu-id="b97b6-113">不使用填充。</span><span class="sxs-lookup"><span data-stu-id="b97b6-113">No padding used.</span></span>|
|<span data-ttu-id="b97b6-114">pkcs1</span><span class="sxs-lookup"><span data-stu-id="b97b6-114">pkcs1</span></span>|<span data-ttu-id="b97b6-115">1</span><span class="sxs-lookup"><span data-stu-id="b97b6-115">1</span></span>|<span data-ttu-id="b97b6-116">使用 PKCS # 1 填充。</span><span class="sxs-lookup"><span data-stu-id="b97b6-116">Use PKCS#1 padding.</span></span>|
|<span data-ttu-id="b97b6-117">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="b97b6-117">oaepSha1</span></span>|<span data-ttu-id="b97b6-118">双面</span><span class="sxs-lookup"><span data-stu-id="b97b6-118">2</span></span>|<span data-ttu-id="b97b6-119">使用 OAEP SHA-1 填充。</span><span class="sxs-lookup"><span data-stu-id="b97b6-119">Use OAEP SHA-1 padding.</span></span>|
|<span data-ttu-id="b97b6-120">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="b97b6-120">oaepSha256</span></span>|<span data-ttu-id="b97b6-121">第三章</span><span class="sxs-lookup"><span data-stu-id="b97b6-121">3</span></span>|<span data-ttu-id="b97b6-122">使用 OAEP SHA-256 填充。</span><span class="sxs-lookup"><span data-stu-id="b97b6-122">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="b97b6-123">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="b97b6-123">oaepSha384</span></span>|<span data-ttu-id="b97b6-124">4</span><span class="sxs-lookup"><span data-stu-id="b97b6-124">4</span></span>|<span data-ttu-id="b97b6-125">使用 OAEP SHA-384 填充。</span><span class="sxs-lookup"><span data-stu-id="b97b6-125">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="b97b6-126">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="b97b6-126">oaepSha512</span></span>|<span data-ttu-id="b97b6-127">5</span><span class="sxs-lookup"><span data-stu-id="b97b6-127">5</span></span>|<span data-ttu-id="b97b6-128">使用 OAEP SHA-512 填充。</span><span class="sxs-lookup"><span data-stu-id="b97b6-128">Use OAEP SHA-512 padding.</span></span>|





