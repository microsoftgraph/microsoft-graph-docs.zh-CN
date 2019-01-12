---
title: safeSearchFilterType 枚举类型
description: 指定需要何种级别的安全搜索 （筛选成人内容）
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 788a266cdd0161ce1cfef426a7fcf4d9726e3324
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964611"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="182af-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="182af-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="182af-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="182af-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="182af-105">指定需要何种级别的安全搜索 （筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="182af-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="182af-106">成员</span><span class="sxs-lookup"><span data-stu-id="182af-106">Members</span></span>
|<span data-ttu-id="182af-107">成员</span><span class="sxs-lookup"><span data-stu-id="182af-107">Member</span></span>|<span data-ttu-id="182af-108">值</span><span class="sxs-lookup"><span data-stu-id="182af-108">Value</span></span>|<span data-ttu-id="182af-109">Description</span><span class="sxs-lookup"><span data-stu-id="182af-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="182af-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="182af-110">userDefined</span></span>|<span data-ttu-id="182af-111">0</span><span class="sxs-lookup"><span data-stu-id="182af-111">0</span></span>|<span data-ttu-id="182af-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="182af-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="182af-113">严格</span><span class="sxs-lookup"><span data-stu-id="182af-113">strict</span></span>|<span data-ttu-id="182af-114">1</span><span class="sxs-lookup"><span data-stu-id="182af-114">1</span></span>|<span data-ttu-id="182af-115">严格，最高针对成人内容筛选。</span><span class="sxs-lookup"><span data-stu-id="182af-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="182af-116">中等</span><span class="sxs-lookup"><span data-stu-id="182af-116">moderate</span></span>|<span data-ttu-id="182af-117">2</span><span class="sxs-lookup"><span data-stu-id="182af-117">2</span></span>|<span data-ttu-id="182af-118">中等筛选成人内容 （有效的搜索结果将不会筛选）。</span><span class="sxs-lookup"><span data-stu-id="182af-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



