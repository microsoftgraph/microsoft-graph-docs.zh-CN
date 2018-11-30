---
title: teamsAsyncOperationType 枚举类型
description: TeamsAsyncOperation 的类型。 将要添加的成员此处为多个异步支持操作。
ms.openlocfilehash: 1911041f50a79874bd1ae2ab41f26b42e85b4250
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041742"
---
# <a name="teamsasyncoperationtype-enum-type"></a><span data-ttu-id="41045-104">teamsAsyncOperationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="41045-104">teamsAsyncOperationType enum type</span></span>

> <span data-ttu-id="41045-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="41045-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41045-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="41045-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41045-107">[TeamsAsyncOperation](teamsasyncoperation.md)的类型。</span><span class="sxs-lookup"><span data-stu-id="41045-107">Types of [teamsAsyncOperation](teamsasyncoperation.md).</span></span> <span data-ttu-id="41045-108">将要添加的成员此处为多个异步支持操作。</span><span class="sxs-lookup"><span data-stu-id="41045-108">Members will be added here as more async operations are supported.</span></span>

## <a name="members"></a><span data-ttu-id="41045-109">成员</span><span class="sxs-lookup"><span data-stu-id="41045-109">Members</span></span>

| <span data-ttu-id="41045-110">成员</span><span class="sxs-lookup"><span data-stu-id="41045-110">Member</span></span> | <span data-ttu-id="41045-111">值</span><span class="sxs-lookup"><span data-stu-id="41045-111">Value</span></span>| <span data-ttu-id="41045-112">说明</span><span class="sxs-lookup"><span data-stu-id="41045-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="41045-113">无效</span><span class="sxs-lookup"><span data-stu-id="41045-113">invalid</span></span>|<span data-ttu-id="41045-114">0</span><span class="sxs-lookup"><span data-stu-id="41045-114">0</span></span>|<span data-ttu-id="41045-115">值无效。</span><span class="sxs-lookup"><span data-stu-id="41045-115">Invalid value.</span></span>|
|<span data-ttu-id="41045-116">cloneTeam</span><span class="sxs-lookup"><span data-stu-id="41045-116">cloneTeam</span></span>|<span data-ttu-id="41045-117">1</span><span class="sxs-lookup"><span data-stu-id="41045-117">1</span></span>|<span data-ttu-id="41045-118">要克隆团队的操作。</span><span class="sxs-lookup"><span data-stu-id="41045-118">Operation to clone a team.</span></span>|
|<span data-ttu-id="41045-119">archiveTeam</span><span class="sxs-lookup"><span data-stu-id="41045-119">archiveTeam</span></span>|<span data-ttu-id="41045-120">2</span><span class="sxs-lookup"><span data-stu-id="41045-120">2</span></span>|<span data-ttu-id="41045-121">若要存档团队的操作。</span><span class="sxs-lookup"><span data-stu-id="41045-121">Operation to archive a team.</span></span>|
|<span data-ttu-id="41045-122">unarchiveTeam</span><span class="sxs-lookup"><span data-stu-id="41045-122">unarchiveTeam</span></span>|<span data-ttu-id="41045-123">3</span><span class="sxs-lookup"><span data-stu-id="41045-123">3</span></span>|<span data-ttu-id="41045-124">若要还原的存档的团队的操作。</span><span class="sxs-lookup"><span data-stu-id="41045-124">Operation to restore an archived team.</span></span>|
|<span data-ttu-id="41045-125">createTeam</span><span class="sxs-lookup"><span data-stu-id="41045-125">createTeam</span></span>|<span data-ttu-id="41045-126">3</span><span class="sxs-lookup"><span data-stu-id="41045-126">3</span></span>|<span data-ttu-id="41045-127">若要从头开始创建团队的操作。</span><span class="sxs-lookup"><span data-stu-id="41045-127">Operation to create a team from scratch.</span></span>|

