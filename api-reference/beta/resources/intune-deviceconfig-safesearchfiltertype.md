---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索 (筛选成人内容)
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f8caa30395fb58eb9fe3e858f5a552c94c42df5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986723"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="ffafa-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ffafa-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="ffafa-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ffafa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffafa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ffafa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffafa-106">指定需要哪个级别的安全搜索 (筛选成人内容)</span><span class="sxs-lookup"><span data-stu-id="ffafa-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="ffafa-107">成员</span><span class="sxs-lookup"><span data-stu-id="ffafa-107">Members</span></span>
|<span data-ttu-id="ffafa-108">成员</span><span class="sxs-lookup"><span data-stu-id="ffafa-108">Member</span></span>|<span data-ttu-id="ffafa-109">值</span><span class="sxs-lookup"><span data-stu-id="ffafa-109">Value</span></span>|<span data-ttu-id="ffafa-110">说明</span><span class="sxs-lookup"><span data-stu-id="ffafa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffafa-111">定制</span><span class="sxs-lookup"><span data-stu-id="ffafa-111">userDefined</span></span>|<span data-ttu-id="ffafa-112">0</span><span class="sxs-lookup"><span data-stu-id="ffafa-112">0</span></span>|<span data-ttu-id="ffafa-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="ffafa-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ffafa-114">全</span><span class="sxs-lookup"><span data-stu-id="ffafa-114">strict</span></span>|<span data-ttu-id="ffafa-115">1</span><span class="sxs-lookup"><span data-stu-id="ffafa-115">1</span></span>|<span data-ttu-id="ffafa-116">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="ffafa-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="ffafa-117">从中</span><span class="sxs-lookup"><span data-stu-id="ffafa-117">moderate</span></span>|<span data-ttu-id="ffafa-118">双面</span><span class="sxs-lookup"><span data-stu-id="ffafa-118">2</span></span>|<span data-ttu-id="ffafa-119">针对成人内容的中等筛选 (将不会筛选有效的搜索结果)。</span><span class="sxs-lookup"><span data-stu-id="ffafa-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





