---
title: ratingCanadaTelevisionType 枚举类型
description: 在加拿大 TV 内容评级标签
author: tfitzmac
ms.openlocfilehash: cf11640b65fd5f0e724c7866dc14322306c3f760
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338708"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="61835-103">ratingCanadaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="61835-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="61835-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="61835-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61835-105">在加拿大 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="61835-105">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="61835-106">成员</span><span class="sxs-lookup"><span data-stu-id="61835-106">Members</span></span>
|<span data-ttu-id="61835-107">成员</span><span class="sxs-lookup"><span data-stu-id="61835-107">Member</span></span>|<span data-ttu-id="61835-108">值</span><span class="sxs-lookup"><span data-stu-id="61835-108">Value</span></span>|<span data-ttu-id="61835-109">说明</span><span class="sxs-lookup"><span data-stu-id="61835-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61835-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="61835-110">allAllowed</span></span>|<span data-ttu-id="61835-111">0</span><span class="sxs-lookup"><span data-stu-id="61835-111">0</span></span>|<span data-ttu-id="61835-112">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="61835-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="61835-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="61835-113">allBlocked</span></span>|<span data-ttu-id="61835-114">1</span><span class="sxs-lookup"><span data-stu-id="61835-114">1</span></span>|<span data-ttu-id="61835-115">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="61835-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="61835-116">children</span><span class="sxs-lookup"><span data-stu-id="61835-116">children</span></span>|<span data-ttu-id="61835-117">2</span><span class="sxs-lookup"><span data-stu-id="61835-117">2</span></span>|<span data-ttu-id="61835-118">C 分类适合子级岁 2 到步骤 7 年</span><span class="sxs-lookup"><span data-stu-id="61835-118">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="61835-119">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="61835-119">childrenAbove8</span></span>|<span data-ttu-id="61835-120">3</span><span class="sxs-lookup"><span data-stu-id="61835-120">3</span></span>|<span data-ttu-id="61835-121">C8 分类适合子级老化 8 +</span><span class="sxs-lookup"><span data-stu-id="61835-121">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="61835-122">常规</span><span class="sxs-lookup"><span data-stu-id="61835-122">general</span></span>|<span data-ttu-id="61835-123">4</span><span class="sxs-lookup"><span data-stu-id="61835-123">4</span></span>|<span data-ttu-id="61835-124">G 分类是适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="61835-124">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="61835-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="61835-125">parentalGuidance</span></span>|<span data-ttu-id="61835-126">5</span><span class="sxs-lookup"><span data-stu-id="61835-126">5</span></span>|<span data-ttu-id="61835-127">PG，家长的指南</span><span class="sxs-lookup"><span data-stu-id="61835-127">PG, Parental Guidance</span></span>|
|<span data-ttu-id="61835-128">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="61835-128">agesAbove14</span></span>|<span data-ttu-id="61835-129">6</span><span class="sxs-lookup"><span data-stu-id="61835-129">6</span></span>|<span data-ttu-id="61835-130">14 + 分类供查看岁 14 及较早</span><span class="sxs-lookup"><span data-stu-id="61835-130">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="61835-131">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="61835-131">agesAbove18</span></span>|<span data-ttu-id="61835-132">7</span><span class="sxs-lookup"><span data-stu-id="61835-132">7</span></span>|<span data-ttu-id="61835-133">18 + 分类供查看岁 18 及较早</span><span class="sxs-lookup"><span data-stu-id="61835-133">The 18+ classification is intended for viewers ages 18 and older</span></span>|



