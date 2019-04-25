---
title: teamsAsyncOperationStatus 枚举类型
description: 描述 teamsAsyncOperation 的当前状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578860"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="210f5-103">teamsAsyncOperationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="210f5-103">teamsAsyncOperationStatus enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="210f5-104">描述[teamsAsyncOperation](teamsasyncoperation.md)的当前状态。</span><span class="sxs-lookup"><span data-stu-id="210f5-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="210f5-105">成员</span><span class="sxs-lookup"><span data-stu-id="210f5-105">Members</span></span>

| <span data-ttu-id="210f5-106">成员</span><span class="sxs-lookup"><span data-stu-id="210f5-106">Member</span></span> | <span data-ttu-id="210f5-107">值</span><span class="sxs-lookup"><span data-stu-id="210f5-107">Value</span></span>| <span data-ttu-id="210f5-108">说明</span><span class="sxs-lookup"><span data-stu-id="210f5-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="210f5-109">无效</span><span class="sxs-lookup"><span data-stu-id="210f5-109">invalid</span></span>|<span data-ttu-id="210f5-110">0</span><span class="sxs-lookup"><span data-stu-id="210f5-110">0</span></span>|<span data-ttu-id="210f5-111">值无效。</span><span class="sxs-lookup"><span data-stu-id="210f5-111">Invalid value.</span></span>|
|<span data-ttu-id="210f5-112">notStarted</span><span class="sxs-lookup"><span data-stu-id="210f5-112">notStarted</span></span>|<span data-ttu-id="210f5-113">1</span><span class="sxs-lookup"><span data-stu-id="210f5-113">1</span></span>|<span data-ttu-id="210f5-114">操作尚未开始。</span><span class="sxs-lookup"><span data-stu-id="210f5-114">The operation has not started.</span></span>|
|<span data-ttu-id="210f5-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="210f5-115">inProgress</span></span>|<span data-ttu-id="210f5-116">2 </span><span class="sxs-lookup"><span data-stu-id="210f5-116">2</span></span>|<span data-ttu-id="210f5-117">操作正在运行。</span><span class="sxs-lookup"><span data-stu-id="210f5-117">The operation is running.</span></span>|
|<span data-ttu-id="210f5-118">完成</span><span class="sxs-lookup"><span data-stu-id="210f5-118">succeeded</span></span>|<span data-ttu-id="210f5-119">3 </span><span class="sxs-lookup"><span data-stu-id="210f5-119">3</span></span>|<span data-ttu-id="210f5-120">操作成功。</span><span class="sxs-lookup"><span data-stu-id="210f5-120">The operation succeeded.</span></span>|
|<span data-ttu-id="210f5-121">未能</span><span class="sxs-lookup"><span data-stu-id="210f5-121">failed</span></span>|<span data-ttu-id="210f5-122">4 </span><span class="sxs-lookup"><span data-stu-id="210f5-122">4</span></span>|<span data-ttu-id="210f5-123">操作失败。</span><span class="sxs-lookup"><span data-stu-id="210f5-123">The operation failed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
