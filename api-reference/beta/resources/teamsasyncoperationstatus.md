---
title: teamsAsyncOperationStatus 枚举类型
description: 介绍 teamsAsyncOperation 的当前状态。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: b6af5c7218a6a9d8c0c5338beb8cdf9944a56c2e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858973"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="f061c-103">teamsAsyncOperationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f061c-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="f061c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f061c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f061c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f061c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f061c-106">介绍[teamsAsyncOperation](teamsasyncoperation.md)的当前状态。</span><span class="sxs-lookup"><span data-stu-id="f061c-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="f061c-107">成员</span><span class="sxs-lookup"><span data-stu-id="f061c-107">Members</span></span>

| <span data-ttu-id="f061c-108">成员</span><span class="sxs-lookup"><span data-stu-id="f061c-108">Member</span></span> | <span data-ttu-id="f061c-109">值</span><span class="sxs-lookup"><span data-stu-id="f061c-109">Value</span></span>| <span data-ttu-id="f061c-110">Description</span><span class="sxs-lookup"><span data-stu-id="f061c-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f061c-111">无效</span><span class="sxs-lookup"><span data-stu-id="f061c-111">invalid</span></span>|<span data-ttu-id="f061c-112">0</span><span class="sxs-lookup"><span data-stu-id="f061c-112">0</span></span>|<span data-ttu-id="f061c-113">值无效。</span><span class="sxs-lookup"><span data-stu-id="f061c-113">Invalid value.</span></span>|
|<span data-ttu-id="f061c-114">为 notStarted</span><span class="sxs-lookup"><span data-stu-id="f061c-114">notStarted</span></span>|<span data-ttu-id="f061c-115">1</span><span class="sxs-lookup"><span data-stu-id="f061c-115">1</span></span>|<span data-ttu-id="f061c-116">尚未开始此操作。</span><span class="sxs-lookup"><span data-stu-id="f061c-116">The operation has not started.</span></span>|
|<span data-ttu-id="f061c-117">正在进行</span><span class="sxs-lookup"><span data-stu-id="f061c-117">inProgress</span></span>|<span data-ttu-id="f061c-118">2</span><span class="sxs-lookup"><span data-stu-id="f061c-118">2</span></span>|<span data-ttu-id="f061c-119">正在运行的操作。</span><span class="sxs-lookup"><span data-stu-id="f061c-119">The operation is running.</span></span>|
|<span data-ttu-id="f061c-120">succeeded</span><span class="sxs-lookup"><span data-stu-id="f061c-120">succeeded</span></span>|<span data-ttu-id="f061c-121">3</span><span class="sxs-lookup"><span data-stu-id="f061c-121">3</span></span>|<span data-ttu-id="f061c-122">操作成功。</span><span class="sxs-lookup"><span data-stu-id="f061c-122">The operation succeeded.</span></span>|
|<span data-ttu-id="f061c-123">failed</span><span class="sxs-lookup"><span data-stu-id="f061c-123">failed</span></span>|<span data-ttu-id="f061c-124">4</span><span class="sxs-lookup"><span data-stu-id="f061c-124">4</span></span>|<span data-ttu-id="f061c-125">操作失败。</span><span class="sxs-lookup"><span data-stu-id="f061c-125">The operation failed.</span></span>|
