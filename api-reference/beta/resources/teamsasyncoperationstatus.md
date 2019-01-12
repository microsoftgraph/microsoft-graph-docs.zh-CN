---
title: teamsAsyncOperationStatus 枚举类型
description: 介绍 teamsAsyncOperation 的当前状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e136d043cf58480d93888374558a1be06ca9053d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914815"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="487d6-103">teamsAsyncOperationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="487d6-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="487d6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="487d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="487d6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="487d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="487d6-106">介绍[teamsAsyncOperation](teamsasyncoperation.md)的当前状态。</span><span class="sxs-lookup"><span data-stu-id="487d6-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="487d6-107">成员</span><span class="sxs-lookup"><span data-stu-id="487d6-107">Members</span></span>

| <span data-ttu-id="487d6-108">成员</span><span class="sxs-lookup"><span data-stu-id="487d6-108">Member</span></span> | <span data-ttu-id="487d6-109">值</span><span class="sxs-lookup"><span data-stu-id="487d6-109">Value</span></span>| <span data-ttu-id="487d6-110">说明</span><span class="sxs-lookup"><span data-stu-id="487d6-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="487d6-111">无效</span><span class="sxs-lookup"><span data-stu-id="487d6-111">invalid</span></span>|<span data-ttu-id="487d6-112">0</span><span class="sxs-lookup"><span data-stu-id="487d6-112">0</span></span>|<span data-ttu-id="487d6-113">值无效。</span><span class="sxs-lookup"><span data-stu-id="487d6-113">Invalid value.</span></span>|
|<span data-ttu-id="487d6-114">为 notStarted</span><span class="sxs-lookup"><span data-stu-id="487d6-114">notStarted</span></span>|<span data-ttu-id="487d6-115">1</span><span class="sxs-lookup"><span data-stu-id="487d6-115">1</span></span>|<span data-ttu-id="487d6-116">尚未开始此操作。</span><span class="sxs-lookup"><span data-stu-id="487d6-116">The operation has not started.</span></span>|
|<span data-ttu-id="487d6-117">正在进行</span><span class="sxs-lookup"><span data-stu-id="487d6-117">inProgress</span></span>|<span data-ttu-id="487d6-118">2</span><span class="sxs-lookup"><span data-stu-id="487d6-118">2</span></span>|<span data-ttu-id="487d6-119">正在运行的操作。</span><span class="sxs-lookup"><span data-stu-id="487d6-119">The operation is running.</span></span>|
|<span data-ttu-id="487d6-120">succeeded</span><span class="sxs-lookup"><span data-stu-id="487d6-120">succeeded</span></span>|<span data-ttu-id="487d6-121">3</span><span class="sxs-lookup"><span data-stu-id="487d6-121">3</span></span>|<span data-ttu-id="487d6-122">操作成功。</span><span class="sxs-lookup"><span data-stu-id="487d6-122">The operation succeeded.</span></span>|
|<span data-ttu-id="487d6-123">failed</span><span class="sxs-lookup"><span data-stu-id="487d6-123">failed</span></span>|<span data-ttu-id="487d6-124">4</span><span class="sxs-lookup"><span data-stu-id="487d6-124">4</span></span>|<span data-ttu-id="487d6-125">操作失败。</span><span class="sxs-lookup"><span data-stu-id="487d6-125">The operation failed.</span></span>|
