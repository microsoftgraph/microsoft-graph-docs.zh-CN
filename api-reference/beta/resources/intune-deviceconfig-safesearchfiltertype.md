---
title: safeSearchFilterType 枚举类型
description: 指定需要何种级别的安全搜索 （筛选成人内容）
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 49252525b3c6bcab6fd79a1ed7c27b3004665fe8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944794"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="9d1d5-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9d1d5-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="9d1d5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9d1d5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d1d5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9d1d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d1d5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9d1d5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d1d5-107">指定需要何种级别的安全搜索 （筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="9d1d5-107">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="9d1d5-108">成员</span><span class="sxs-lookup"><span data-stu-id="9d1d5-108">Members</span></span>
|<span data-ttu-id="9d1d5-109">成员</span><span class="sxs-lookup"><span data-stu-id="9d1d5-109">Member</span></span>|<span data-ttu-id="9d1d5-110">值</span><span class="sxs-lookup"><span data-stu-id="9d1d5-110">Value</span></span>|<span data-ttu-id="9d1d5-111">Description</span><span class="sxs-lookup"><span data-stu-id="9d1d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d1d5-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="9d1d5-112">userDefined</span></span>|<span data-ttu-id="9d1d5-113">0</span><span class="sxs-lookup"><span data-stu-id="9d1d5-113">0</span></span>|<span data-ttu-id="9d1d5-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="9d1d5-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="9d1d5-115">严格</span><span class="sxs-lookup"><span data-stu-id="9d1d5-115">strict</span></span>|<span data-ttu-id="9d1d5-116">1</span><span class="sxs-lookup"><span data-stu-id="9d1d5-116">1</span></span>|<span data-ttu-id="9d1d5-117">严格，最高针对成人内容筛选。</span><span class="sxs-lookup"><span data-stu-id="9d1d5-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="9d1d5-118">中等</span><span class="sxs-lookup"><span data-stu-id="9d1d5-118">moderate</span></span>|<span data-ttu-id="9d1d5-119">2</span><span class="sxs-lookup"><span data-stu-id="9d1d5-119">2</span></span>|<span data-ttu-id="9d1d5-120">中等筛选成人内容 （有效的搜索结果将不会筛选）。</span><span class="sxs-lookup"><span data-stu-id="9d1d5-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





