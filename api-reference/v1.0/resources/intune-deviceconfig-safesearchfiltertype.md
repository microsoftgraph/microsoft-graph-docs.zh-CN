---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索（筛选成人内容）
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c8ef86709169448d58bde53507747377526c38ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530466"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="f62e4-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f62e4-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="f62e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f62e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f62e4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f62e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f62e4-106">指定需要哪个级别的安全搜索（筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="f62e4-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="f62e4-107">成员</span><span class="sxs-lookup"><span data-stu-id="f62e4-107">Members</span></span>
|<span data-ttu-id="f62e4-108">成员</span><span class="sxs-lookup"><span data-stu-id="f62e4-108">Member</span></span>|<span data-ttu-id="f62e4-109">值</span><span class="sxs-lookup"><span data-stu-id="f62e4-109">Value</span></span>|<span data-ttu-id="f62e4-110">说明</span><span class="sxs-lookup"><span data-stu-id="f62e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f62e4-111">定制</span><span class="sxs-lookup"><span data-stu-id="f62e4-111">userDefined</span></span>|<span data-ttu-id="f62e4-112">0</span><span class="sxs-lookup"><span data-stu-id="f62e4-112">0</span></span>|<span data-ttu-id="f62e4-113">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="f62e4-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f62e4-114">全</span><span class="sxs-lookup"><span data-stu-id="f62e4-114">strict</span></span>|<span data-ttu-id="f62e4-115">1 </span><span class="sxs-lookup"><span data-stu-id="f62e4-115">1</span></span>|<span data-ttu-id="f62e4-116">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="f62e4-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="f62e4-117">从中</span><span class="sxs-lookup"><span data-stu-id="f62e4-117">moderate</span></span>|<span data-ttu-id="f62e4-118">2 </span><span class="sxs-lookup"><span data-stu-id="f62e4-118">2</span></span>|<span data-ttu-id="f62e4-119">针对成人内容的中等筛选（将不会筛选有效的搜索结果）。</span><span class="sxs-lookup"><span data-stu-id="f62e4-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




