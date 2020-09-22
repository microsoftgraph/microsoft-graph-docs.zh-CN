---
title: safeSearchFilterType 枚举类型
description: 指定 (筛选成人内容) 所需的安全搜索级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 194344e7403e678edaf2a4a04eab9c9564ddc9a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091633"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="33126-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="33126-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="33126-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33126-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33126-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="33126-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33126-106">指定 (筛选成人内容) 所需的安全搜索级别</span><span class="sxs-lookup"><span data-stu-id="33126-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="33126-107">成员</span><span class="sxs-lookup"><span data-stu-id="33126-107">Members</span></span>
|<span data-ttu-id="33126-108">成员</span><span class="sxs-lookup"><span data-stu-id="33126-108">Member</span></span>|<span data-ttu-id="33126-109">值</span><span class="sxs-lookup"><span data-stu-id="33126-109">Value</span></span>|<span data-ttu-id="33126-110">说明</span><span class="sxs-lookup"><span data-stu-id="33126-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33126-111">定制</span><span class="sxs-lookup"><span data-stu-id="33126-111">userDefined</span></span>|<span data-ttu-id="33126-112">0</span><span class="sxs-lookup"><span data-stu-id="33126-112">0</span></span>|<span data-ttu-id="33126-113">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="33126-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="33126-114">全</span><span class="sxs-lookup"><span data-stu-id="33126-114">strict</span></span>|<span data-ttu-id="33126-115">1 </span><span class="sxs-lookup"><span data-stu-id="33126-115">1</span></span>|<span data-ttu-id="33126-116">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="33126-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="33126-117">从中</span><span class="sxs-lookup"><span data-stu-id="33126-117">moderate</span></span>|<span data-ttu-id="33126-118">2 </span><span class="sxs-lookup"><span data-stu-id="33126-118">2</span></span>|<span data-ttu-id="33126-119">针对成人内容的中等筛选 (将不会) 筛选有效的搜索结果。</span><span class="sxs-lookup"><span data-stu-id="33126-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|









