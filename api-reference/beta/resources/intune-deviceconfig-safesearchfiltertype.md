---
title: safeSearchFilterType 枚举类型
description: 指定 (筛选成人内容) 所需的安全搜索级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2e043979f3f57b16ad4d2bb62b1c7d8710889f3b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48710025"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="198ec-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="198ec-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="198ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="198ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="198ec-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="198ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="198ec-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="198ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="198ec-107">指定 (筛选成人内容) 所需的安全搜索级别</span><span class="sxs-lookup"><span data-stu-id="198ec-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="198ec-108">成员</span><span class="sxs-lookup"><span data-stu-id="198ec-108">Members</span></span>
|<span data-ttu-id="198ec-109">成员</span><span class="sxs-lookup"><span data-stu-id="198ec-109">Member</span></span>|<span data-ttu-id="198ec-110">值</span><span class="sxs-lookup"><span data-stu-id="198ec-110">Value</span></span>|<span data-ttu-id="198ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="198ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="198ec-112">定制</span><span class="sxs-lookup"><span data-stu-id="198ec-112">userDefined</span></span>|<span data-ttu-id="198ec-113">0</span><span class="sxs-lookup"><span data-stu-id="198ec-113">0</span></span>|<span data-ttu-id="198ec-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="198ec-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="198ec-115">全</span><span class="sxs-lookup"><span data-stu-id="198ec-115">strict</span></span>|<span data-ttu-id="198ec-116">1</span><span class="sxs-lookup"><span data-stu-id="198ec-116">1</span></span>|<span data-ttu-id="198ec-117">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="198ec-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="198ec-118">从中</span><span class="sxs-lookup"><span data-stu-id="198ec-118">moderate</span></span>|<span data-ttu-id="198ec-119">双面</span><span class="sxs-lookup"><span data-stu-id="198ec-119">2</span></span>|<span data-ttu-id="198ec-120">针对成人内容的中等筛选 (将不会) 筛选有效的搜索结果。</span><span class="sxs-lookup"><span data-stu-id="198ec-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





