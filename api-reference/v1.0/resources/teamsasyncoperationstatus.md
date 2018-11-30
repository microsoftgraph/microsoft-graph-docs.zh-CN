---
title: teamsAsyncOperationStatus 枚举类型
description: 介绍 teamsAsyncOperation 的当前状态。
ms.openlocfilehash: 10f8dbbc80150892b37d0d5a05affc2fb13f9a5a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008017"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="2f903-103">teamsAsyncOperationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2f903-103">teamsAsyncOperationStatus enum type</span></span>



<span data-ttu-id="2f903-104">介绍[teamsAsyncOperation](teamsasyncoperation.md)的当前状态。</span><span class="sxs-lookup"><span data-stu-id="2f903-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="2f903-105">成员</span><span class="sxs-lookup"><span data-stu-id="2f903-105">Members</span></span>

| <span data-ttu-id="2f903-106">成员</span><span class="sxs-lookup"><span data-stu-id="2f903-106">Member</span></span> | <span data-ttu-id="2f903-107">值</span><span class="sxs-lookup"><span data-stu-id="2f903-107">Value</span></span>| <span data-ttu-id="2f903-108">说明</span><span class="sxs-lookup"><span data-stu-id="2f903-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2f903-109">无效</span><span class="sxs-lookup"><span data-stu-id="2f903-109">invalid</span></span>|<span data-ttu-id="2f903-110">0</span><span class="sxs-lookup"><span data-stu-id="2f903-110">0</span></span>|<span data-ttu-id="2f903-111">值无效。</span><span class="sxs-lookup"><span data-stu-id="2f903-111">Invalid value.</span></span>|
|<span data-ttu-id="2f903-112">为 notStarted</span><span class="sxs-lookup"><span data-stu-id="2f903-112">notStarted</span></span>|<span data-ttu-id="2f903-113">1</span><span class="sxs-lookup"><span data-stu-id="2f903-113">1</span></span>|<span data-ttu-id="2f903-114">尚未开始此操作。</span><span class="sxs-lookup"><span data-stu-id="2f903-114">The operation has not started.</span></span>|
|<span data-ttu-id="2f903-115">正在进行</span><span class="sxs-lookup"><span data-stu-id="2f903-115">inProgress</span></span>|<span data-ttu-id="2f903-116">2</span><span class="sxs-lookup"><span data-stu-id="2f903-116">2</span></span>|<span data-ttu-id="2f903-117">正在运行的操作。</span><span class="sxs-lookup"><span data-stu-id="2f903-117">The operation is running.</span></span>|
|<span data-ttu-id="2f903-118">succeeded</span><span class="sxs-lookup"><span data-stu-id="2f903-118">succeeded</span></span>|<span data-ttu-id="2f903-119">3</span><span class="sxs-lookup"><span data-stu-id="2f903-119">3</span></span>|<span data-ttu-id="2f903-120">操作成功。</span><span class="sxs-lookup"><span data-stu-id="2f903-120">The operation succeeded.</span></span>|
|<span data-ttu-id="2f903-121">failed</span><span class="sxs-lookup"><span data-stu-id="2f903-121">failed</span></span>|<span data-ttu-id="2f903-122">4</span><span class="sxs-lookup"><span data-stu-id="2f903-122">4</span></span>|<span data-ttu-id="2f903-123">操作失败。</span><span class="sxs-lookup"><span data-stu-id="2f903-123">The operation failed.</span></span>|