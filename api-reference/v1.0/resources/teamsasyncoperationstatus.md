---
title: teamsAsyncOperationStatus 枚举类型
description: 介绍 teamsAsyncOperation 的当前状态。
author: nkramer
ms.openlocfilehash: fbf66ac0c93fd616793ebb4dc62fb63a2559374f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309966"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="1f7cf-103">teamsAsyncOperationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1f7cf-103">teamsAsyncOperationStatus enum type</span></span>



<span data-ttu-id="1f7cf-104">介绍[teamsAsyncOperation](teamsasyncoperation.md)的当前状态。</span><span class="sxs-lookup"><span data-stu-id="1f7cf-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="1f7cf-105">成员</span><span class="sxs-lookup"><span data-stu-id="1f7cf-105">Members</span></span>

| <span data-ttu-id="1f7cf-106">成员</span><span class="sxs-lookup"><span data-stu-id="1f7cf-106">Member</span></span> | <span data-ttu-id="1f7cf-107">值</span><span class="sxs-lookup"><span data-stu-id="1f7cf-107">Value</span></span>| <span data-ttu-id="1f7cf-108">说明</span><span class="sxs-lookup"><span data-stu-id="1f7cf-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1f7cf-109">无效</span><span class="sxs-lookup"><span data-stu-id="1f7cf-109">invalid</span></span>|<span data-ttu-id="1f7cf-110">0</span><span class="sxs-lookup"><span data-stu-id="1f7cf-110">0</span></span>|<span data-ttu-id="1f7cf-111">值无效。</span><span class="sxs-lookup"><span data-stu-id="1f7cf-111">Invalid value.</span></span>|
|<span data-ttu-id="1f7cf-112">为 notStarted</span><span class="sxs-lookup"><span data-stu-id="1f7cf-112">notStarted</span></span>|<span data-ttu-id="1f7cf-113">1</span><span class="sxs-lookup"><span data-stu-id="1f7cf-113">1</span></span>|<span data-ttu-id="1f7cf-114">尚未开始此操作。</span><span class="sxs-lookup"><span data-stu-id="1f7cf-114">The operation has not started.</span></span>|
|<span data-ttu-id="1f7cf-115">正在进行</span><span class="sxs-lookup"><span data-stu-id="1f7cf-115">inProgress</span></span>|<span data-ttu-id="1f7cf-116">2</span><span class="sxs-lookup"><span data-stu-id="1f7cf-116">2</span></span>|<span data-ttu-id="1f7cf-117">正在运行的操作。</span><span class="sxs-lookup"><span data-stu-id="1f7cf-117">The operation is running.</span></span>|
|<span data-ttu-id="1f7cf-118">succeeded</span><span class="sxs-lookup"><span data-stu-id="1f7cf-118">succeeded</span></span>|<span data-ttu-id="1f7cf-119">3</span><span class="sxs-lookup"><span data-stu-id="1f7cf-119">3</span></span>|<span data-ttu-id="1f7cf-120">操作成功。</span><span class="sxs-lookup"><span data-stu-id="1f7cf-120">The operation succeeded.</span></span>|
|<span data-ttu-id="1f7cf-121">failed</span><span class="sxs-lookup"><span data-stu-id="1f7cf-121">failed</span></span>|<span data-ttu-id="1f7cf-122">4</span><span class="sxs-lookup"><span data-stu-id="1f7cf-122">4</span></span>|<span data-ttu-id="1f7cf-123">操作失败。</span><span class="sxs-lookup"><span data-stu-id="1f7cf-123">The operation failed.</span></span>|