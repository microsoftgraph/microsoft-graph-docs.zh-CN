---
title: ratingAppsType 枚举类型
description: 分级如媒体内容中所示的应用程序
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 709734a36010ded195a93b383adefc80f729c4fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953404"
---
# <a name="ratingappstype-enum-type"></a><span data-ttu-id="d3b2a-103">ratingAppsType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d3b2a-103">ratingAppsType enum type</span></span>

> <span data-ttu-id="d3b2a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d3b2a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3b2a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d3b2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3b2a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d3b2a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3b2a-107">分级如媒体内容中所示的应用程序</span><span class="sxs-lookup"><span data-stu-id="d3b2a-107">Apps rating as in media content</span></span>
## <a name="members"></a><span data-ttu-id="d3b2a-108">成员</span><span class="sxs-lookup"><span data-stu-id="d3b2a-108">Members</span></span>
|<span data-ttu-id="d3b2a-109">成员</span><span class="sxs-lookup"><span data-stu-id="d3b2a-109">Member</span></span>|<span data-ttu-id="d3b2a-110">值</span><span class="sxs-lookup"><span data-stu-id="d3b2a-110">Value</span></span>|<span data-ttu-id="d3b2a-111">说明</span><span class="sxs-lookup"><span data-stu-id="d3b2a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3b2a-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="d3b2a-112">allAllowed</span></span>|<span data-ttu-id="d3b2a-113">0</span><span class="sxs-lookup"><span data-stu-id="d3b2a-113">0</span></span>|<span data-ttu-id="d3b2a-114">默认值，允许所有应用程序内容</span><span class="sxs-lookup"><span data-stu-id="d3b2a-114">Default value, allow all apps content</span></span>|
|<span data-ttu-id="d3b2a-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="d3b2a-115">allBlocked</span></span>|<span data-ttu-id="d3b2a-116">1</span><span class="sxs-lookup"><span data-stu-id="d3b2a-116">1</span></span>|<span data-ttu-id="d3b2a-117">不允许任何应用程序内容</span><span class="sxs-lookup"><span data-stu-id="d3b2a-117">Do not allow any apps content</span></span>|
|<span data-ttu-id="d3b2a-118">agesAbove4</span><span class="sxs-lookup"><span data-stu-id="d3b2a-118">agesAbove4</span></span>|<span data-ttu-id="d3b2a-119">2</span><span class="sxs-lookup"><span data-stu-id="d3b2a-119">2</span></span>|<span data-ttu-id="d3b2a-120">4 + age 4 及以上</span><span class="sxs-lookup"><span data-stu-id="d3b2a-120">4+, age 4 and above</span></span>|
|<span data-ttu-id="d3b2a-121">agesAbove9</span><span class="sxs-lookup"><span data-stu-id="d3b2a-121">agesAbove9</span></span>|<span data-ttu-id="d3b2a-122">3</span><span class="sxs-lookup"><span data-stu-id="d3b2a-122">3</span></span>|<span data-ttu-id="d3b2a-123">9 + age 9 及以上</span><span class="sxs-lookup"><span data-stu-id="d3b2a-123">9+, age 9 and above</span></span>|
|<span data-ttu-id="d3b2a-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="d3b2a-124">agesAbove12</span></span>|<span data-ttu-id="d3b2a-125">4</span><span class="sxs-lookup"><span data-stu-id="d3b2a-125">4</span></span>|<span data-ttu-id="d3b2a-126">12 + age 12 及以上</span><span class="sxs-lookup"><span data-stu-id="d3b2a-126">12+, age 12 and above</span></span> |
|<span data-ttu-id="d3b2a-127">agesAbove17</span><span class="sxs-lookup"><span data-stu-id="d3b2a-127">agesAbove17</span></span>|<span data-ttu-id="d3b2a-128">5</span><span class="sxs-lookup"><span data-stu-id="d3b2a-128">5</span></span>|<span data-ttu-id="d3b2a-129">17 + age 17 及以上</span><span class="sxs-lookup"><span data-stu-id="d3b2a-129">17+, age 17 and above</span></span>|





