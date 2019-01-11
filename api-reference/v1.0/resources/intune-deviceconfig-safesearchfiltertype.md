---
title: safeSearchFilterType 枚举类型
description: 指定需要何种级别的安全搜索 （筛选成人内容）
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 28aea918c35bb9d90f514e4a8838f219c212405b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830854"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="26de9-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="26de9-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="26de9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="26de9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26de9-105">指定需要何种级别的安全搜索 （筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="26de9-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="26de9-106">成员</span><span class="sxs-lookup"><span data-stu-id="26de9-106">Members</span></span>
|<span data-ttu-id="26de9-107">成员</span><span class="sxs-lookup"><span data-stu-id="26de9-107">Member</span></span>|<span data-ttu-id="26de9-108">值</span><span class="sxs-lookup"><span data-stu-id="26de9-108">Value</span></span>|<span data-ttu-id="26de9-109">Description</span><span class="sxs-lookup"><span data-stu-id="26de9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26de9-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="26de9-110">userDefined</span></span>|<span data-ttu-id="26de9-111">0</span><span class="sxs-lookup"><span data-stu-id="26de9-111">0</span></span>|<span data-ttu-id="26de9-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="26de9-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="26de9-113">严格</span><span class="sxs-lookup"><span data-stu-id="26de9-113">strict</span></span>|<span data-ttu-id="26de9-114">1</span><span class="sxs-lookup"><span data-stu-id="26de9-114">1</span></span>|<span data-ttu-id="26de9-115">严格，最高针对成人内容筛选。</span><span class="sxs-lookup"><span data-stu-id="26de9-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="26de9-116">中等</span><span class="sxs-lookup"><span data-stu-id="26de9-116">moderate</span></span>|<span data-ttu-id="26de9-117">2</span><span class="sxs-lookup"><span data-stu-id="26de9-117">2</span></span>|<span data-ttu-id="26de9-118">中等筛选成人内容 （有效的搜索结果将不会筛选）。</span><span class="sxs-lookup"><span data-stu-id="26de9-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



