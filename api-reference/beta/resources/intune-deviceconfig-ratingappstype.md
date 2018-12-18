---
title: ratingAppsType 枚举类型
description: 分级如媒体内容中所示的应用程序
author: tfitzmac
ms.openlocfilehash: fa9a70128347201657dfa0d5de6044142b37525d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345526"
---
# <a name="ratingappstype-enum-type"></a><span data-ttu-id="14d97-103">ratingAppsType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="14d97-103">ratingAppsType enum type</span></span>

> <span data-ttu-id="14d97-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="14d97-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14d97-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="14d97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14d97-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="14d97-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14d97-107">分级如媒体内容中所示的应用程序</span><span class="sxs-lookup"><span data-stu-id="14d97-107">Apps rating as in media content</span></span>
## <a name="members"></a><span data-ttu-id="14d97-108">成员</span><span class="sxs-lookup"><span data-stu-id="14d97-108">Members</span></span>
|<span data-ttu-id="14d97-109">成员</span><span class="sxs-lookup"><span data-stu-id="14d97-109">Member</span></span>|<span data-ttu-id="14d97-110">值</span><span class="sxs-lookup"><span data-stu-id="14d97-110">Value</span></span>|<span data-ttu-id="14d97-111">说明</span><span class="sxs-lookup"><span data-stu-id="14d97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14d97-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="14d97-112">allAllowed</span></span>|<span data-ttu-id="14d97-113">0</span><span class="sxs-lookup"><span data-stu-id="14d97-113">0</span></span>|<span data-ttu-id="14d97-114">默认值，允许所有应用程序内容</span><span class="sxs-lookup"><span data-stu-id="14d97-114">Default value, allow all apps content</span></span>|
|<span data-ttu-id="14d97-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="14d97-115">allBlocked</span></span>|<span data-ttu-id="14d97-116">1</span><span class="sxs-lookup"><span data-stu-id="14d97-116">1</span></span>|<span data-ttu-id="14d97-117">不允许任何应用程序内容</span><span class="sxs-lookup"><span data-stu-id="14d97-117">Do not allow any apps content</span></span>|
|<span data-ttu-id="14d97-118">agesAbove4</span><span class="sxs-lookup"><span data-stu-id="14d97-118">agesAbove4</span></span>|<span data-ttu-id="14d97-119">2</span><span class="sxs-lookup"><span data-stu-id="14d97-119">2</span></span>|<span data-ttu-id="14d97-120">4 + age 4 及以上</span><span class="sxs-lookup"><span data-stu-id="14d97-120">4+, age 4 and above</span></span>|
|<span data-ttu-id="14d97-121">agesAbove9</span><span class="sxs-lookup"><span data-stu-id="14d97-121">agesAbove9</span></span>|<span data-ttu-id="14d97-122">3</span><span class="sxs-lookup"><span data-stu-id="14d97-122">3</span></span>|<span data-ttu-id="14d97-123">9 + age 9 及以上</span><span class="sxs-lookup"><span data-stu-id="14d97-123">9+, age 9 and above</span></span>|
|<span data-ttu-id="14d97-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="14d97-124">agesAbove12</span></span>|<span data-ttu-id="14d97-125">4</span><span class="sxs-lookup"><span data-stu-id="14d97-125">4</span></span>|<span data-ttu-id="14d97-126">12 + age 12 及以上</span><span class="sxs-lookup"><span data-stu-id="14d97-126">12+, age 12 and above</span></span> |
|<span data-ttu-id="14d97-127">agesAbove17</span><span class="sxs-lookup"><span data-stu-id="14d97-127">agesAbove17</span></span>|<span data-ttu-id="14d97-128">5</span><span class="sxs-lookup"><span data-stu-id="14d97-128">5</span></span>|<span data-ttu-id="14d97-129">17 + age 17 及以上</span><span class="sxs-lookup"><span data-stu-id="14d97-129">17+, age 17 and above</span></span>|





