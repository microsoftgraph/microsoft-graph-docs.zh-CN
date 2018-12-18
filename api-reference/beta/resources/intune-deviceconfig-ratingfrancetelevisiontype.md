---
title: ratingFranceTelevisionType 枚举类型
description: 在法国 TV 内容评级标签
author: tfitzmac
ms.openlocfilehash: f202b2e942e36e7c13052643a31ee0a984723f5d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312213"
---
# <a name="ratingfrancetelevisiontype-enum-type"></a><span data-ttu-id="f6d8f-103">ratingFranceTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f6d8f-103">ratingFranceTelevisionType enum type</span></span>

> <span data-ttu-id="f6d8f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f6d8f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6d8f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f6d8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6d8f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f6d8f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6d8f-107">在法国 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="f6d8f-107">TV content rating labels in France</span></span>
## <a name="members"></a><span data-ttu-id="f6d8f-108">成员</span><span class="sxs-lookup"><span data-stu-id="f6d8f-108">Members</span></span>
|<span data-ttu-id="f6d8f-109">成员</span><span class="sxs-lookup"><span data-stu-id="f6d8f-109">Member</span></span>|<span data-ttu-id="f6d8f-110">值</span><span class="sxs-lookup"><span data-stu-id="f6d8f-110">Value</span></span>|<span data-ttu-id="f6d8f-111">说明</span><span class="sxs-lookup"><span data-stu-id="f6d8f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6d8f-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="f6d8f-112">allAllowed</span></span>|<span data-ttu-id="f6d8f-113">0</span><span class="sxs-lookup"><span data-stu-id="f6d8f-113">0</span></span>|<span data-ttu-id="f6d8f-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="f6d8f-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="f6d8f-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="f6d8f-115">allBlocked</span></span>|<span data-ttu-id="f6d8f-116">1</span><span class="sxs-lookup"><span data-stu-id="f6d8f-116">1</span></span>|<span data-ttu-id="f6d8f-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="f6d8f-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="f6d8f-118">agesAbove10</span><span class="sxs-lookup"><span data-stu-id="f6d8f-118">agesAbove10</span></span>|<span data-ttu-id="f6d8f-119">2</span><span class="sxs-lookup"><span data-stu-id="f6d8f-119">2</span></span>|<span data-ttu-id="f6d8f-120">-10 分类不建议对子级下 10</span><span class="sxs-lookup"><span data-stu-id="f6d8f-120">The -10 classification is not recommended for children under 10</span></span>|
|<span data-ttu-id="f6d8f-121">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="f6d8f-121">agesAbove12</span></span>|<span data-ttu-id="f6d8f-122">3</span><span class="sxs-lookup"><span data-stu-id="f6d8f-122">3</span></span>|<span data-ttu-id="f6d8f-123">-12 分类不建议对子级下 12</span><span class="sxs-lookup"><span data-stu-id="f6d8f-123">The -12 classification is not recommended for children under 12</span></span>|
|<span data-ttu-id="f6d8f-124">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="f6d8f-124">agesAbove16</span></span>|<span data-ttu-id="f6d8f-125">4</span><span class="sxs-lookup"><span data-stu-id="f6d8f-125">4</span></span>|<span data-ttu-id="f6d8f-126">-16 分类不建议对子级下 16</span><span class="sxs-lookup"><span data-stu-id="f6d8f-126">The -16 classification is not recommended for children under 16</span></span>|
|<span data-ttu-id="f6d8f-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="f6d8f-127">agesAbove18</span></span>|<span data-ttu-id="f6d8f-128">5</span><span class="sxs-lookup"><span data-stu-id="f6d8f-128">5</span></span>|<span data-ttu-id="f6d8f-129">-18 分类不建议对下 18 的人员</span><span class="sxs-lookup"><span data-stu-id="f6d8f-129">The -18 classification is not recommended for persons under 18</span></span>|





