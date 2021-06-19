---
title: teamsAsyncOperationType 枚举类型
description: teamsAsyncOperation 的类型。 由于支持更多异步操作，因此将在此处添加成员。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: enumPageType
ms.openlocfilehash: 5765fabd5e9b13f040c6f7b189a31223414fc0a0
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030829"
---
# <a name="teamsasyncoperationtype-enum-type"></a><span data-ttu-id="ac845-104">teamsAsyncOperationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ac845-104">teamsAsyncOperationType enum type</span></span>

<span data-ttu-id="ac845-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac845-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac845-106">[teamsAsyncOperation 的类型](teamsasyncoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="ac845-106">Types of [teamsAsyncOperation](teamsasyncoperation.md).</span></span> <span data-ttu-id="ac845-107">由于支持更多异步操作，因此将在此处添加成员。</span><span class="sxs-lookup"><span data-stu-id="ac845-107">Members will be added here as more async operations are supported.</span></span>

## <a name="members"></a><span data-ttu-id="ac845-108">成员</span><span class="sxs-lookup"><span data-stu-id="ac845-108">Members</span></span>

| <span data-ttu-id="ac845-109">成员</span><span class="sxs-lookup"><span data-stu-id="ac845-109">Member</span></span> | <span data-ttu-id="ac845-110">值</span><span class="sxs-lookup"><span data-stu-id="ac845-110">Value</span></span>| <span data-ttu-id="ac845-111">说明</span><span class="sxs-lookup"><span data-stu-id="ac845-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ac845-112">无效</span><span class="sxs-lookup"><span data-stu-id="ac845-112">invalid</span></span>|<span data-ttu-id="ac845-113">0</span><span class="sxs-lookup"><span data-stu-id="ac845-113">0</span></span>|<span data-ttu-id="ac845-114">值无效。</span><span class="sxs-lookup"><span data-stu-id="ac845-114">Invalid value.</span></span>|
|<span data-ttu-id="ac845-115">cloneTeam</span><span class="sxs-lookup"><span data-stu-id="ac845-115">cloneTeam</span></span>|<span data-ttu-id="ac845-116">1</span><span class="sxs-lookup"><span data-stu-id="ac845-116">1</span></span>|<span data-ttu-id="ac845-117">克隆团队的操作。</span><span class="sxs-lookup"><span data-stu-id="ac845-117">Operation to clone a team.</span></span>|
|<span data-ttu-id="ac845-118">archiveTeam</span><span class="sxs-lookup"><span data-stu-id="ac845-118">archiveTeam</span></span>|<span data-ttu-id="ac845-119">2</span><span class="sxs-lookup"><span data-stu-id="ac845-119">2</span></span>|<span data-ttu-id="ac845-120">存档团队的操作。</span><span class="sxs-lookup"><span data-stu-id="ac845-120">Operation to archive a team.</span></span>|
|<span data-ttu-id="ac845-121">unarchiveTeam</span><span class="sxs-lookup"><span data-stu-id="ac845-121">unarchiveTeam</span></span>|<span data-ttu-id="ac845-122">3</span><span class="sxs-lookup"><span data-stu-id="ac845-122">3</span></span>|<span data-ttu-id="ac845-123">还原存档团队的操作。</span><span class="sxs-lookup"><span data-stu-id="ac845-123">Operation to restore an archived team.</span></span>|
|<span data-ttu-id="ac845-124">createTeam</span><span class="sxs-lookup"><span data-stu-id="ac845-124">createTeam</span></span>|<span data-ttu-id="ac845-125">4 </span><span class="sxs-lookup"><span data-stu-id="ac845-125">4</span></span>|<span data-ttu-id="ac845-126">从头开始创建团队的操作。</span><span class="sxs-lookup"><span data-stu-id="ac845-126">Operation to create a team from scratch.</span></span>|
|<span data-ttu-id="ac845-127">createChat</span><span class="sxs-lookup"><span data-stu-id="ac845-127">createChat</span></span>|<span data-ttu-id="ac845-128">5 </span><span class="sxs-lookup"><span data-stu-id="ac845-128">5</span></span>|<span data-ttu-id="ac845-129">从头开始创建聊天的操作。</span><span class="sxs-lookup"><span data-stu-id="ac845-129">Operation to create a chat from scratch.</span></span>|
