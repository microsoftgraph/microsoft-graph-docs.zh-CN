---
title: teamsAsyncOperationStatus 枚举类型
description: 介绍 teamsAsyncOperation 的当前状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511707"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="123b2-103">teamsAsyncOperationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="123b2-103">teamsAsyncOperationStatus enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="123b2-104">介绍[teamsAsyncOperation](teamsasyncoperation.md)的当前状态。</span><span class="sxs-lookup"><span data-stu-id="123b2-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="123b2-105">成员</span><span class="sxs-lookup"><span data-stu-id="123b2-105">Members</span></span>

| <span data-ttu-id="123b2-106">成员</span><span class="sxs-lookup"><span data-stu-id="123b2-106">Member</span></span> | <span data-ttu-id="123b2-107">值</span><span class="sxs-lookup"><span data-stu-id="123b2-107">Value</span></span>| <span data-ttu-id="123b2-108">说明</span><span class="sxs-lookup"><span data-stu-id="123b2-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="123b2-109">Invalid</span><span class="sxs-lookup"><span data-stu-id="123b2-109">invalid</span></span>|<span data-ttu-id="123b2-110">0%</span><span class="sxs-lookup"><span data-stu-id="123b2-110">0</span></span>|<span data-ttu-id="123b2-111">值无效</span><span class="sxs-lookup"><span data-stu-id="123b2-111">Invalid value.</span></span>|
|<span data-ttu-id="123b2-112">NotStarted</span><span class="sxs-lookup"><span data-stu-id="123b2-112">notStarted</span></span>|<span data-ttu-id="123b2-113">$1</span><span class="sxs-lookup"><span data-stu-id="123b2-113">1</span></span>|<span data-ttu-id="123b2-114">尚未开始此操作。</span><span class="sxs-lookup"><span data-stu-id="123b2-114">The operation has not started.</span></span>|
|<span data-ttu-id="123b2-115">InProgress</span><span class="sxs-lookup"><span data-stu-id="123b2-115">inProgress</span></span>|<span data-ttu-id="123b2-116">-2</span><span class="sxs-lookup"><span data-stu-id="123b2-116">2</span></span>|<span data-ttu-id="123b2-117">正在运行的操作。</span><span class="sxs-lookup"><span data-stu-id="123b2-117">The operation is running.</span></span>|
|<span data-ttu-id="123b2-118">succeeded</span><span class="sxs-lookup"><span data-stu-id="123b2-118">succeeded</span></span>|<span data-ttu-id="123b2-119">-3</span><span class="sxs-lookup"><span data-stu-id="123b2-119">3</span></span>|<span data-ttu-id="123b2-120">操作成功。</span><span class="sxs-lookup"><span data-stu-id="123b2-120">The operation succeeded.</span></span>|
|<span data-ttu-id="123b2-121">failed</span><span class="sxs-lookup"><span data-stu-id="123b2-121">failed</span></span>|<span data-ttu-id="123b2-122">-4</span><span class="sxs-lookup"><span data-stu-id="123b2-122">4</span></span>|<span data-ttu-id="123b2-123">操作失败。</span><span class="sxs-lookup"><span data-stu-id="123b2-123">The operation failed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
