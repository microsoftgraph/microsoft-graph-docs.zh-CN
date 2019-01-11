---
title: 成员
description: '介绍团队的可见性。 '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 21f53b1d7631cde46f1bd70afcbb1346f9199d9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884537"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="afe08-103">teamVisibilityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="afe08-103">teamVisibilityType enum type</span></span>

> <span data-ttu-id="afe08-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="afe08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afe08-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="afe08-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="afe08-106">介绍[团队](../resources/team.md)的可见性。</span><span class="sxs-lookup"><span data-stu-id="afe08-106">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="afe08-107">成员</span><span class="sxs-lookup"><span data-stu-id="afe08-107">Members</span></span>

| <span data-ttu-id="afe08-108">成员</span><span class="sxs-lookup"><span data-stu-id="afe08-108">Member</span></span> | <span data-ttu-id="afe08-109">值</span><span class="sxs-lookup"><span data-stu-id="afe08-109">Value</span></span>| <span data-ttu-id="afe08-110">Description</span><span class="sxs-lookup"><span data-stu-id="afe08-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="afe08-111">专用</span><span class="sxs-lookup"><span data-stu-id="afe08-111">private</span></span>|<span data-ttu-id="afe08-112">0</span><span class="sxs-lookup"><span data-stu-id="afe08-112">0</span></span>|<span data-ttu-id="afe08-113">任何人都能看到团队，但只有所有者可以将用户添加到团队。</span><span class="sxs-lookup"><span data-stu-id="afe08-113">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="afe08-114">公开</span><span class="sxs-lookup"><span data-stu-id="afe08-114">public</span></span>|<span data-ttu-id="afe08-115">1</span><span class="sxs-lookup"><span data-stu-id="afe08-115">1</span></span>|<span data-ttu-id="afe08-116">任何人都可以加入团队。</span><span class="sxs-lookup"><span data-stu-id="afe08-116">Anyone can join the team.</span></span>|
