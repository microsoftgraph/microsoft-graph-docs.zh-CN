---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索 (筛选成人内容)
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c88542d6d06f623d20a294cc49aff321692c75a6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027851"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="c1c8b-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c1c8b-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="c1c8b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1c8b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1c8b-105">指定需要哪个级别的安全搜索 (筛选成人内容)</span><span class="sxs-lookup"><span data-stu-id="c1c8b-105">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="c1c8b-106">成员</span><span class="sxs-lookup"><span data-stu-id="c1c8b-106">Members</span></span>
|<span data-ttu-id="c1c8b-107">成员</span><span class="sxs-lookup"><span data-stu-id="c1c8b-107">Member</span></span>|<span data-ttu-id="c1c8b-108">值</span><span class="sxs-lookup"><span data-stu-id="c1c8b-108">Value</span></span>|<span data-ttu-id="c1c8b-109">说明</span><span class="sxs-lookup"><span data-stu-id="c1c8b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c8b-110">定制</span><span class="sxs-lookup"><span data-stu-id="c1c8b-110">userDefined</span></span>|<span data-ttu-id="c1c8b-111">0</span><span class="sxs-lookup"><span data-stu-id="c1c8b-111">0</span></span>|<span data-ttu-id="c1c8b-112">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="c1c8b-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c1c8b-113">全</span><span class="sxs-lookup"><span data-stu-id="c1c8b-113">strict</span></span>|<span data-ttu-id="c1c8b-114">1</span><span class="sxs-lookup"><span data-stu-id="c1c8b-114">1</span></span>|<span data-ttu-id="c1c8b-115">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="c1c8b-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="c1c8b-116">从中</span><span class="sxs-lookup"><span data-stu-id="c1c8b-116">moderate</span></span>|<span data-ttu-id="c1c8b-117">双面</span><span class="sxs-lookup"><span data-stu-id="c1c8b-117">2</span></span>|<span data-ttu-id="c1c8b-118">针对成人内容的中等筛选 (将不会筛选有效的搜索结果)。</span><span class="sxs-lookup"><span data-stu-id="c1c8b-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



