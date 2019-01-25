---
title: teamsAsyncOperationType 枚举类型
description: TeamsAsyncOperation 的类型。 将要添加的成员此处为多个异步支持操作。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4de95db194bf41939521b53f06614b46b6afae99
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516565"
---
# <a name="teamsasyncoperationtype-enum-type"></a><span data-ttu-id="91d17-104">teamsAsyncOperationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="91d17-104">teamsAsyncOperationType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91d17-105">[TeamsAsyncOperation](teamsasyncoperation.md)的类型。</span><span class="sxs-lookup"><span data-stu-id="91d17-105">Types of [teamsAsyncOperation](teamsasyncoperation.md).</span></span> <span data-ttu-id="91d17-106">将要添加的成员此处为多个异步支持操作。</span><span class="sxs-lookup"><span data-stu-id="91d17-106">Members will be added here as more async operations are supported.</span></span>

## <a name="members"></a><span data-ttu-id="91d17-107">成员</span><span class="sxs-lookup"><span data-stu-id="91d17-107">Members</span></span>

| <span data-ttu-id="91d17-108">成员</span><span class="sxs-lookup"><span data-stu-id="91d17-108">Member</span></span> | <span data-ttu-id="91d17-109">值</span><span class="sxs-lookup"><span data-stu-id="91d17-109">Value</span></span>| <span data-ttu-id="91d17-110">说明</span><span class="sxs-lookup"><span data-stu-id="91d17-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="91d17-111">Invalid</span><span class="sxs-lookup"><span data-stu-id="91d17-111">invalid</span></span>|<span data-ttu-id="91d17-112">0%</span><span class="sxs-lookup"><span data-stu-id="91d17-112">0</span></span>|<span data-ttu-id="91d17-113">值无效</span><span class="sxs-lookup"><span data-stu-id="91d17-113">Invalid value.</span></span>|
|<span data-ttu-id="91d17-114">cloneTeam</span><span class="sxs-lookup"><span data-stu-id="91d17-114">cloneTeam</span></span>|<span data-ttu-id="91d17-115">$1</span><span class="sxs-lookup"><span data-stu-id="91d17-115">1</span></span>|<span data-ttu-id="91d17-116">要克隆团队的操作。</span><span class="sxs-lookup"><span data-stu-id="91d17-116">Operation to clone a team.</span></span>|
|<span data-ttu-id="91d17-117">archiveTeam</span><span class="sxs-lookup"><span data-stu-id="91d17-117">archiveTeam</span></span>|<span data-ttu-id="91d17-118">-2</span><span class="sxs-lookup"><span data-stu-id="91d17-118">2</span></span>|<span data-ttu-id="91d17-119">若要存档团队的操作。</span><span class="sxs-lookup"><span data-stu-id="91d17-119">Operation to archive a team.</span></span>|
|<span data-ttu-id="91d17-120">unarchiveTeam</span><span class="sxs-lookup"><span data-stu-id="91d17-120">unarchiveTeam</span></span>|<span data-ttu-id="91d17-121">-3</span><span class="sxs-lookup"><span data-stu-id="91d17-121">3</span></span>|<span data-ttu-id="91d17-122">若要还原的存档的团队的操作。</span><span class="sxs-lookup"><span data-stu-id="91d17-122">Operation to restore an archived team.</span></span>|
|<span data-ttu-id="91d17-123">createTeam</span><span class="sxs-lookup"><span data-stu-id="91d17-123">createTeam</span></span>|<span data-ttu-id="91d17-124">-3</span><span class="sxs-lookup"><span data-stu-id="91d17-124">3</span></span>|<span data-ttu-id="91d17-125">若要从头开始创建团队的操作。</span><span class="sxs-lookup"><span data-stu-id="91d17-125">Operation to create a team from scratch.</span></span>|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
