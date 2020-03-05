---
title: teamsAsyncOperationStatus 枚举类型
description: 描述 teamsAsyncOperation 的当前状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2c82065c789847d3e2a11947dcf921b12c55530e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519895"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="e6f85-103">teamsAsyncOperationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e6f85-103">teamsAsyncOperationStatus enum type</span></span>

<span data-ttu-id="e6f85-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e6f85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6f85-105">描述[teamsAsyncOperation](teamsasyncoperation.md)的当前状态。</span><span class="sxs-lookup"><span data-stu-id="e6f85-105">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="e6f85-106">成员</span><span class="sxs-lookup"><span data-stu-id="e6f85-106">Members</span></span>

| <span data-ttu-id="e6f85-107">成员</span><span class="sxs-lookup"><span data-stu-id="e6f85-107">Member</span></span> | <span data-ttu-id="e6f85-108">值</span><span class="sxs-lookup"><span data-stu-id="e6f85-108">Value</span></span>| <span data-ttu-id="e6f85-109">说明</span><span class="sxs-lookup"><span data-stu-id="e6f85-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e6f85-110">无效</span><span class="sxs-lookup"><span data-stu-id="e6f85-110">invalid</span></span>|<span data-ttu-id="e6f85-111">0</span><span class="sxs-lookup"><span data-stu-id="e6f85-111">0</span></span>|<span data-ttu-id="e6f85-112">值无效。</span><span class="sxs-lookup"><span data-stu-id="e6f85-112">Invalid value.</span></span>|
|<span data-ttu-id="e6f85-113">notStarted</span><span class="sxs-lookup"><span data-stu-id="e6f85-113">notStarted</span></span>|<span data-ttu-id="e6f85-114">1 </span><span class="sxs-lookup"><span data-stu-id="e6f85-114">1</span></span>|<span data-ttu-id="e6f85-115">操作尚未开始。</span><span class="sxs-lookup"><span data-stu-id="e6f85-115">The operation has not started.</span></span>|
|<span data-ttu-id="e6f85-116">inProgress</span><span class="sxs-lookup"><span data-stu-id="e6f85-116">inProgress</span></span>|<span data-ttu-id="e6f85-117">2 </span><span class="sxs-lookup"><span data-stu-id="e6f85-117">2</span></span>|<span data-ttu-id="e6f85-118">操作正在运行。</span><span class="sxs-lookup"><span data-stu-id="e6f85-118">The operation is running.</span></span>|
|<span data-ttu-id="e6f85-119">完成</span><span class="sxs-lookup"><span data-stu-id="e6f85-119">succeeded</span></span>|<span data-ttu-id="e6f85-120">3 </span><span class="sxs-lookup"><span data-stu-id="e6f85-120">3</span></span>|<span data-ttu-id="e6f85-121">操作成功。</span><span class="sxs-lookup"><span data-stu-id="e6f85-121">The operation succeeded.</span></span>|
|<span data-ttu-id="e6f85-122">未能</span><span class="sxs-lookup"><span data-stu-id="e6f85-122">failed</span></span>|<span data-ttu-id="e6f85-123">4 </span><span class="sxs-lookup"><span data-stu-id="e6f85-123">4</span></span>|<span data-ttu-id="e6f85-124">操作失败。</span><span class="sxs-lookup"><span data-stu-id="e6f85-124">The operation failed.</span></span>|
