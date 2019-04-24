---
title: teamsAsyncOperationType 枚举类型
description: teamsAsyncOperation 的类型。 将在此处添加成员, 因为支持更多的异步操作。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3866c41b74fc6748479099d43b268afa115dde67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462233"
---
# <a name="teamsasyncoperationtype-enum-type"></a><span data-ttu-id="1e3d5-104">teamsAsyncOperationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1e3d5-104">teamsAsyncOperationType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e3d5-105">[teamsAsyncOperation](teamsasyncoperation.md)的类型。</span><span class="sxs-lookup"><span data-stu-id="1e3d5-105">Types of [teamsAsyncOperation](teamsasyncoperation.md).</span></span> <span data-ttu-id="1e3d5-106">将在此处添加成员, 因为支持更多的异步操作。</span><span class="sxs-lookup"><span data-stu-id="1e3d5-106">Members will be added here as more async operations are supported.</span></span>

## <a name="members"></a><span data-ttu-id="1e3d5-107">成员</span><span class="sxs-lookup"><span data-stu-id="1e3d5-107">Members</span></span>

| <span data-ttu-id="1e3d5-108">成员</span><span class="sxs-lookup"><span data-stu-id="1e3d5-108">Member</span></span> | <span data-ttu-id="1e3d5-109">值</span><span class="sxs-lookup"><span data-stu-id="1e3d5-109">Value</span></span>| <span data-ttu-id="1e3d5-110">说明</span><span class="sxs-lookup"><span data-stu-id="1e3d5-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1e3d5-111">无效</span><span class="sxs-lookup"><span data-stu-id="1e3d5-111">invalid</span></span>|<span data-ttu-id="1e3d5-112">0</span><span class="sxs-lookup"><span data-stu-id="1e3d5-112">0</span></span>|<span data-ttu-id="1e3d5-113">值无效。</span><span class="sxs-lookup"><span data-stu-id="1e3d5-113">Invalid value.</span></span>|
|<span data-ttu-id="1e3d5-114">cloneTeam</span><span class="sxs-lookup"><span data-stu-id="1e3d5-114">cloneTeam</span></span>|<span data-ttu-id="1e3d5-115">1</span><span class="sxs-lookup"><span data-stu-id="1e3d5-115">1</span></span>|<span data-ttu-id="1e3d5-116">克隆团队的操作。</span><span class="sxs-lookup"><span data-stu-id="1e3d5-116">Operation to clone a team.</span></span>|
|<span data-ttu-id="1e3d5-117">archiveTeam</span><span class="sxs-lookup"><span data-stu-id="1e3d5-117">archiveTeam</span></span>|<span data-ttu-id="1e3d5-118">2 </span><span class="sxs-lookup"><span data-stu-id="1e3d5-118">2</span></span>|<span data-ttu-id="1e3d5-119">存档团队的操作。</span><span class="sxs-lookup"><span data-stu-id="1e3d5-119">Operation to archive a team.</span></span>|
|<span data-ttu-id="1e3d5-120">unarchiveTeam</span><span class="sxs-lookup"><span data-stu-id="1e3d5-120">unarchiveTeam</span></span>|<span data-ttu-id="1e3d5-121">3 </span><span class="sxs-lookup"><span data-stu-id="1e3d5-121">3</span></span>|<span data-ttu-id="1e3d5-122">还原存档团队的操作。</span><span class="sxs-lookup"><span data-stu-id="1e3d5-122">Operation to restore an archived team.</span></span>|
|<span data-ttu-id="1e3d5-123">createTeam</span><span class="sxs-lookup"><span data-stu-id="1e3d5-123">createTeam</span></span>|<span data-ttu-id="1e3d5-124">3 </span><span class="sxs-lookup"><span data-stu-id="1e3d5-124">3</span></span>|<span data-ttu-id="1e3d5-125">从头开始创建团队的操作。</span><span class="sxs-lookup"><span data-stu-id="1e3d5-125">Operation to create a team from scratch.</span></span>|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
