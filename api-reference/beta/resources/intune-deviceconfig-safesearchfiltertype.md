---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索 (筛选成人内容)
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 564e641fcdc7e0d06d48666881fc3bcedfe3505c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573212"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="35775-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="35775-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="35775-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35775-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35775-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35775-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35775-106">指定需要哪个级别的安全搜索 (筛选成人内容)</span><span class="sxs-lookup"><span data-stu-id="35775-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="35775-107">成员</span><span class="sxs-lookup"><span data-stu-id="35775-107">Members</span></span>
|<span data-ttu-id="35775-108">成员</span><span class="sxs-lookup"><span data-stu-id="35775-108">Member</span></span>|<span data-ttu-id="35775-109">值</span><span class="sxs-lookup"><span data-stu-id="35775-109">Value</span></span>|<span data-ttu-id="35775-110">说明</span><span class="sxs-lookup"><span data-stu-id="35775-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35775-111">定制</span><span class="sxs-lookup"><span data-stu-id="35775-111">userDefined</span></span>|<span data-ttu-id="35775-112">0</span><span class="sxs-lookup"><span data-stu-id="35775-112">0</span></span>|<span data-ttu-id="35775-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="35775-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="35775-114">全</span><span class="sxs-lookup"><span data-stu-id="35775-114">strict</span></span>|<span data-ttu-id="35775-115">1</span><span class="sxs-lookup"><span data-stu-id="35775-115">1</span></span>|<span data-ttu-id="35775-116">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="35775-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="35775-117">从中</span><span class="sxs-lookup"><span data-stu-id="35775-117">moderate</span></span>|<span data-ttu-id="35775-118">2 </span><span class="sxs-lookup"><span data-stu-id="35775-118">2</span></span>|<span data-ttu-id="35775-119">针对成人内容的中等筛选 (将不会筛选有效的搜索结果)。</span><span class="sxs-lookup"><span data-stu-id="35775-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





