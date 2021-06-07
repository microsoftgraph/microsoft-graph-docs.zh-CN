---
title: safeSearchFilterType 枚举类型
description: 指定筛选成人内容 (需要的安全搜索) 级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 60463edb06c961e7911b5391ea8b3e4e8f1150ec
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754697"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="be5d0-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="be5d0-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="be5d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be5d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be5d0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be5d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be5d0-106">指定筛选成人内容 (需要的安全搜索) 级别</span><span class="sxs-lookup"><span data-stu-id="be5d0-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="be5d0-107">成员</span><span class="sxs-lookup"><span data-stu-id="be5d0-107">Members</span></span>
|<span data-ttu-id="be5d0-108">成员</span><span class="sxs-lookup"><span data-stu-id="be5d0-108">Member</span></span>|<span data-ttu-id="be5d0-109">值</span><span class="sxs-lookup"><span data-stu-id="be5d0-109">Value</span></span>|<span data-ttu-id="be5d0-110">Description</span><span class="sxs-lookup"><span data-stu-id="be5d0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be5d0-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="be5d0-111">userDefined</span></span>|<span data-ttu-id="be5d0-112">0</span><span class="sxs-lookup"><span data-stu-id="be5d0-112">0</span></span>|<span data-ttu-id="be5d0-113">用户定义，默认值，无意图。</span><span class="sxs-lookup"><span data-stu-id="be5d0-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="be5d0-114">strict</span><span class="sxs-lookup"><span data-stu-id="be5d0-114">strict</span></span>|<span data-ttu-id="be5d0-115">1</span><span class="sxs-lookup"><span data-stu-id="be5d0-115">1</span></span>|<span data-ttu-id="be5d0-116">对成人内容进行严格、最高的筛选。</span><span class="sxs-lookup"><span data-stu-id="be5d0-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="be5d0-117">中等</span><span class="sxs-lookup"><span data-stu-id="be5d0-117">moderate</span></span>|<span data-ttu-id="be5d0-118">2</span><span class="sxs-lookup"><span data-stu-id="be5d0-118">2</span></span>|<span data-ttu-id="be5d0-119">对成人内容进行适量 (将不会筛选出有效的) 。</span><span class="sxs-lookup"><span data-stu-id="be5d0-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




