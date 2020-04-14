---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索（筛选成人内容）
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8585745d2f4e9c529e6ef56c9ce209b1da67f2ac
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444875"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="2baa3-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2baa3-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="2baa3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2baa3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2baa3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2baa3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2baa3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2baa3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2baa3-107">指定需要哪个级别的安全搜索（筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="2baa3-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="2baa3-108">成员</span><span class="sxs-lookup"><span data-stu-id="2baa3-108">Members</span></span>
|<span data-ttu-id="2baa3-109">成员</span><span class="sxs-lookup"><span data-stu-id="2baa3-109">Member</span></span>|<span data-ttu-id="2baa3-110">值</span><span class="sxs-lookup"><span data-stu-id="2baa3-110">Value</span></span>|<span data-ttu-id="2baa3-111">说明</span><span class="sxs-lookup"><span data-stu-id="2baa3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2baa3-112">定制</span><span class="sxs-lookup"><span data-stu-id="2baa3-112">userDefined</span></span>|<span data-ttu-id="2baa3-113">0</span><span class="sxs-lookup"><span data-stu-id="2baa3-113">0</span></span>|<span data-ttu-id="2baa3-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="2baa3-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2baa3-115">全</span><span class="sxs-lookup"><span data-stu-id="2baa3-115">strict</span></span>|<span data-ttu-id="2baa3-116">1</span><span class="sxs-lookup"><span data-stu-id="2baa3-116">1</span></span>|<span data-ttu-id="2baa3-117">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="2baa3-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="2baa3-118">从中</span><span class="sxs-lookup"><span data-stu-id="2baa3-118">moderate</span></span>|<span data-ttu-id="2baa3-119">双面</span><span class="sxs-lookup"><span data-stu-id="2baa3-119">2</span></span>|<span data-ttu-id="2baa3-120">针对成人内容的中等筛选（将不会筛选有效的搜索结果）。</span><span class="sxs-lookup"><span data-stu-id="2baa3-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



