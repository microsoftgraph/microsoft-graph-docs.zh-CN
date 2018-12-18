---
title: safeSearchFilterType 枚举类型
description: 指定需要何种级别的安全搜索 （筛选成人内容）
author: tfitzmac
ms.openlocfilehash: eb0c7cfb862364ddc4703c89d19ea844ada6466d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343195"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="e9471-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e9471-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="e9471-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e9471-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9471-105">指定需要何种级别的安全搜索 （筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="e9471-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="e9471-106">成员</span><span class="sxs-lookup"><span data-stu-id="e9471-106">Members</span></span>
|<span data-ttu-id="e9471-107">成员</span><span class="sxs-lookup"><span data-stu-id="e9471-107">Member</span></span>|<span data-ttu-id="e9471-108">值</span><span class="sxs-lookup"><span data-stu-id="e9471-108">Value</span></span>|<span data-ttu-id="e9471-109">说明</span><span class="sxs-lookup"><span data-stu-id="e9471-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9471-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="e9471-110">userDefined</span></span>|<span data-ttu-id="e9471-111">0</span><span class="sxs-lookup"><span data-stu-id="e9471-111">0</span></span>|<span data-ttu-id="e9471-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="e9471-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e9471-113">严格</span><span class="sxs-lookup"><span data-stu-id="e9471-113">strict</span></span>|<span data-ttu-id="e9471-114">1</span><span class="sxs-lookup"><span data-stu-id="e9471-114">1</span></span>|<span data-ttu-id="e9471-115">严格，最高针对成人内容筛选。</span><span class="sxs-lookup"><span data-stu-id="e9471-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="e9471-116">中等</span><span class="sxs-lookup"><span data-stu-id="e9471-116">moderate</span></span>|<span data-ttu-id="e9471-117">2</span><span class="sxs-lookup"><span data-stu-id="e9471-117">2</span></span>|<span data-ttu-id="e9471-118">中等筛选成人内容 （有效的搜索结果将不会筛选）。</span><span class="sxs-lookup"><span data-stu-id="e9471-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



