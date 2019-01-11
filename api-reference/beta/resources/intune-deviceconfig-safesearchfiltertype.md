---
title: safeSearchFilterType 枚举类型
description: 指定需要何种级别的安全搜索 （筛选成人内容）
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 477f0b52342ca1b27d844a5f03aedd806cdd8b5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875829"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="95ace-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="95ace-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="95ace-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="95ace-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95ace-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="95ace-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95ace-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="95ace-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95ace-107">指定需要何种级别的安全搜索 （筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="95ace-107">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="95ace-108">成员</span><span class="sxs-lookup"><span data-stu-id="95ace-108">Members</span></span>
|<span data-ttu-id="95ace-109">成员</span><span class="sxs-lookup"><span data-stu-id="95ace-109">Member</span></span>|<span data-ttu-id="95ace-110">值</span><span class="sxs-lookup"><span data-stu-id="95ace-110">Value</span></span>|<span data-ttu-id="95ace-111">Description</span><span class="sxs-lookup"><span data-stu-id="95ace-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95ace-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="95ace-112">userDefined</span></span>|<span data-ttu-id="95ace-113">0</span><span class="sxs-lookup"><span data-stu-id="95ace-113">0</span></span>|<span data-ttu-id="95ace-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="95ace-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="95ace-115">严格</span><span class="sxs-lookup"><span data-stu-id="95ace-115">strict</span></span>|<span data-ttu-id="95ace-116">1</span><span class="sxs-lookup"><span data-stu-id="95ace-116">1</span></span>|<span data-ttu-id="95ace-117">严格，最高针对成人内容筛选。</span><span class="sxs-lookup"><span data-stu-id="95ace-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="95ace-118">中等</span><span class="sxs-lookup"><span data-stu-id="95ace-118">moderate</span></span>|<span data-ttu-id="95ace-119">2</span><span class="sxs-lookup"><span data-stu-id="95ace-119">2</span></span>|<span data-ttu-id="95ace-120">中等筛选成人内容 （有效的搜索结果将不会筛选）。</span><span class="sxs-lookup"><span data-stu-id="95ace-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





