---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索 (筛选成人内容)
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c82f80f6081f57a88fcdf26f7639277d72b5e0d8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534897"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="2c706-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2c706-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="2c706-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c706-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c706-105">指定需要哪个级别的安全搜索 (筛选成人内容)</span><span class="sxs-lookup"><span data-stu-id="2c706-105">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="2c706-106">成员</span><span class="sxs-lookup"><span data-stu-id="2c706-106">Members</span></span>
|<span data-ttu-id="2c706-107">成员</span><span class="sxs-lookup"><span data-stu-id="2c706-107">Member</span></span>|<span data-ttu-id="2c706-108">值</span><span class="sxs-lookup"><span data-stu-id="2c706-108">Value</span></span>|<span data-ttu-id="2c706-109">说明</span><span class="sxs-lookup"><span data-stu-id="2c706-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c706-110">定制</span><span class="sxs-lookup"><span data-stu-id="2c706-110">userDefined</span></span>|<span data-ttu-id="2c706-111">0</span><span class="sxs-lookup"><span data-stu-id="2c706-111">0</span></span>|<span data-ttu-id="2c706-112">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="2c706-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2c706-113">全</span><span class="sxs-lookup"><span data-stu-id="2c706-113">strict</span></span>|<span data-ttu-id="2c706-114">1</span><span class="sxs-lookup"><span data-stu-id="2c706-114">1</span></span>|<span data-ttu-id="2c706-115">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="2c706-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="2c706-116">从中</span><span class="sxs-lookup"><span data-stu-id="2c706-116">moderate</span></span>|<span data-ttu-id="2c706-117">2 </span><span class="sxs-lookup"><span data-stu-id="2c706-117">2</span></span>|<span data-ttu-id="2c706-118">针对成人内容的中等筛选 (将不会筛选有效的搜索结果)。</span><span class="sxs-lookup"><span data-stu-id="2c706-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



