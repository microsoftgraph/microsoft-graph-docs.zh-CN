---
title: safeSearchFilterType 枚举类型
description: 指定需要哪个级别的安全搜索（筛选成人内容）
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 92cad118957ea383b886cccc8fb29066e8b2fd20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529436"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="1601f-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1601f-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="1601f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1601f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1601f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1601f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1601f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1601f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1601f-107">指定需要哪个级别的安全搜索（筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="1601f-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="1601f-108">成员</span><span class="sxs-lookup"><span data-stu-id="1601f-108">Members</span></span>
|<span data-ttu-id="1601f-109">成员</span><span class="sxs-lookup"><span data-stu-id="1601f-109">Member</span></span>|<span data-ttu-id="1601f-110">值</span><span class="sxs-lookup"><span data-stu-id="1601f-110">Value</span></span>|<span data-ttu-id="1601f-111">说明</span><span class="sxs-lookup"><span data-stu-id="1601f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1601f-112">定制</span><span class="sxs-lookup"><span data-stu-id="1601f-112">userDefined</span></span>|<span data-ttu-id="1601f-113">0</span><span class="sxs-lookup"><span data-stu-id="1601f-113">0</span></span>|<span data-ttu-id="1601f-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="1601f-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="1601f-115">全</span><span class="sxs-lookup"><span data-stu-id="1601f-115">strict</span></span>|<span data-ttu-id="1601f-116">1 </span><span class="sxs-lookup"><span data-stu-id="1601f-116">1</span></span>|<span data-ttu-id="1601f-117">对成人内容严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="1601f-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="1601f-118">从中</span><span class="sxs-lookup"><span data-stu-id="1601f-118">moderate</span></span>|<span data-ttu-id="1601f-119">2 </span><span class="sxs-lookup"><span data-stu-id="1601f-119">2</span></span>|<span data-ttu-id="1601f-120">针对成人内容的中等筛选（将不会筛选有效的搜索结果）。</span><span class="sxs-lookup"><span data-stu-id="1601f-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



