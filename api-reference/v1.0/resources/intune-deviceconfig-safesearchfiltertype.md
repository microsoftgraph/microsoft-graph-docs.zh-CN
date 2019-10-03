---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索（筛选成人内容）
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7df74b38fcf5fe0ad62f93f9e4245638016f2189
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367747"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="ee1b2-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ee1b2-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="ee1b2-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ee1b2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee1b2-105">指定需要哪个级别的安全搜索（筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="ee1b2-105">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="ee1b2-106">成员</span><span class="sxs-lookup"><span data-stu-id="ee1b2-106">Members</span></span>
|<span data-ttu-id="ee1b2-107">成员</span><span class="sxs-lookup"><span data-stu-id="ee1b2-107">Member</span></span>|<span data-ttu-id="ee1b2-108">值</span><span class="sxs-lookup"><span data-stu-id="ee1b2-108">Value</span></span>|<span data-ttu-id="ee1b2-109">说明</span><span class="sxs-lookup"><span data-stu-id="ee1b2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee1b2-110">定制</span><span class="sxs-lookup"><span data-stu-id="ee1b2-110">userDefined</span></span>|<span data-ttu-id="ee1b2-111">0</span><span class="sxs-lookup"><span data-stu-id="ee1b2-111">0</span></span>|<span data-ttu-id="ee1b2-112">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="ee1b2-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ee1b2-113">全</span><span class="sxs-lookup"><span data-stu-id="ee1b2-113">strict</span></span>|<span data-ttu-id="ee1b2-114">1</span><span class="sxs-lookup"><span data-stu-id="ee1b2-114">1</span></span>|<span data-ttu-id="ee1b2-115">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="ee1b2-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="ee1b2-116">从中</span><span class="sxs-lookup"><span data-stu-id="ee1b2-116">moderate</span></span>|<span data-ttu-id="ee1b2-117">双面</span><span class="sxs-lookup"><span data-stu-id="ee1b2-117">2</span></span>|<span data-ttu-id="ee1b2-118">针对成人内容的中等筛选（将不会筛选有效的搜索结果）。</span><span class="sxs-lookup"><span data-stu-id="ee1b2-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




