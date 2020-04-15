---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索（筛选成人内容）
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7b9beb5f96cfbbe900c7aa655150d62497629a3e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472672"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="e54a9-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e54a9-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="e54a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e54a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e54a9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e54a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e54a9-106">指定需要哪个级别的安全搜索（筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="e54a9-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="e54a9-107">成员</span><span class="sxs-lookup"><span data-stu-id="e54a9-107">Members</span></span>
|<span data-ttu-id="e54a9-108">成员</span><span class="sxs-lookup"><span data-stu-id="e54a9-108">Member</span></span>|<span data-ttu-id="e54a9-109">值</span><span class="sxs-lookup"><span data-stu-id="e54a9-109">Value</span></span>|<span data-ttu-id="e54a9-110">说明</span><span class="sxs-lookup"><span data-stu-id="e54a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e54a9-111">定制</span><span class="sxs-lookup"><span data-stu-id="e54a9-111">userDefined</span></span>|<span data-ttu-id="e54a9-112">0</span><span class="sxs-lookup"><span data-stu-id="e54a9-112">0</span></span>|<span data-ttu-id="e54a9-113">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="e54a9-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e54a9-114">全</span><span class="sxs-lookup"><span data-stu-id="e54a9-114">strict</span></span>|<span data-ttu-id="e54a9-115">1</span><span class="sxs-lookup"><span data-stu-id="e54a9-115">1</span></span>|<span data-ttu-id="e54a9-116">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="e54a9-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="e54a9-117">从中</span><span class="sxs-lookup"><span data-stu-id="e54a9-117">moderate</span></span>|<span data-ttu-id="e54a9-118">双面</span><span class="sxs-lookup"><span data-stu-id="e54a9-118">2</span></span>|<span data-ttu-id="e54a9-119">针对成人内容的中等筛选（将不会筛选有效的搜索结果）。</span><span class="sxs-lookup"><span data-stu-id="e54a9-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|







