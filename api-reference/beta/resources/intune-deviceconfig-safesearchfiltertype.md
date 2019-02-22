---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索 (筛选成人内容)
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 196131eb11efad25a4b2fa541bf1b20d85dda33e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140171"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="22ef2-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="22ef2-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="22ef2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22ef2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22ef2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22ef2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22ef2-106">指定需要哪个级别的安全搜索 (筛选成人内容)</span><span class="sxs-lookup"><span data-stu-id="22ef2-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="22ef2-107">成员</span><span class="sxs-lookup"><span data-stu-id="22ef2-107">Members</span></span>
|<span data-ttu-id="22ef2-108">成员</span><span class="sxs-lookup"><span data-stu-id="22ef2-108">Member</span></span>|<span data-ttu-id="22ef2-109">值</span><span class="sxs-lookup"><span data-stu-id="22ef2-109">Value</span></span>|<span data-ttu-id="22ef2-110">说明</span><span class="sxs-lookup"><span data-stu-id="22ef2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22ef2-111">定制</span><span class="sxs-lookup"><span data-stu-id="22ef2-111">userDefined</span></span>|<span data-ttu-id="22ef2-112">0</span><span class="sxs-lookup"><span data-stu-id="22ef2-112">0</span></span>|<span data-ttu-id="22ef2-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="22ef2-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="22ef2-114">全</span><span class="sxs-lookup"><span data-stu-id="22ef2-114">strict</span></span>|<span data-ttu-id="22ef2-115">1</span><span class="sxs-lookup"><span data-stu-id="22ef2-115">1</span></span>|<span data-ttu-id="22ef2-116">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="22ef2-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="22ef2-117">从中</span><span class="sxs-lookup"><span data-stu-id="22ef2-117">moderate</span></span>|<span data-ttu-id="22ef2-118">双面</span><span class="sxs-lookup"><span data-stu-id="22ef2-118">2</span></span>|<span data-ttu-id="22ef2-119">针对成人内容的中等筛选 (将不会筛选有效的搜索结果)。</span><span class="sxs-lookup"><span data-stu-id="22ef2-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




