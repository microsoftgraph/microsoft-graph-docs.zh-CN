---
title: conditionalAccess 资源类型
description: '**conditionalaccess** 资源是 Conditinal Access 对象模型的入口点。 它不包含任何可用属性。'
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3683965cda79f003cb5e548101272d869be902b8
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547411"
---
# <a name="conditionalaccess-resource-type"></a><span data-ttu-id="2f091-104">conditionalaccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f091-104">conditionalaccess resource type</span></span>

<span data-ttu-id="2f091-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f091-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f091-106">**conditionalAccess** 资源是条件访问对象模型的入口点。</span><span class="sxs-lookup"><span data-stu-id="2f091-106">The **conditionalAccess** resource is the entry point for the Conditional Access object model.</span></span> <span data-ttu-id="2f091-107">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="2f091-107">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="2f091-108">方法</span><span class="sxs-lookup"><span data-stu-id="2f091-108">Methods</span></span>

| <span data-ttu-id="2f091-109">方法</span><span class="sxs-lookup"><span data-stu-id="2f091-109">Method</span></span>           | <span data-ttu-id="2f091-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2f091-110">Return Type</span></span>    |<span data-ttu-id="2f091-111">说明</span><span class="sxs-lookup"><span data-stu-id="2f091-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f091-112">创建 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2f091-112">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) |[<span data-ttu-id="2f091-113">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2f091-113">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md)| <span data-ttu-id="2f091-114">通过发布到 **conditionalAccessPolicy** 集合创建新的 conditionalAccessPolicy。</span><span class="sxs-lookup"><span data-stu-id="2f091-114">Create a new **conditionalAccessPolicy** by posting to the conditionalAccessPolicy collection.</span></span>|
|[<span data-ttu-id="2f091-115">创建 namedLocations</span><span class="sxs-lookup"><span data-stu-id="2f091-115">Create namedLocations</span></span>](../api/conditionalaccessroot-post-namedlocations.md) |[<span data-ttu-id="2f091-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="2f091-116">namedLocation</span></span>](namedlocation.md)| <span data-ttu-id="2f091-117">通过发布到 **namedLocations** 集合创建新的 namedLocations。</span><span class="sxs-lookup"><span data-stu-id="2f091-117">Create a new **namedLocations** by posting to the namedLocations collection.</span></span>|
|[<span data-ttu-id="2f091-118">创建 authenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="2f091-118">Create authenticationContextClassReferences</span></span>](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md)|[<span data-ttu-id="2f091-119">authenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="2f091-119">authenticationContextClassReferences</span></span>](authenticationcontextclassreference.md)|<span data-ttu-id="2f091-120">通过发布到 **authenticationContextClassReferences** 集合创建新的 authenticationContextClassReferences。</span><span class="sxs-lookup"><span data-stu-id="2f091-120">Create a new **authenticationContextClassReferences** by posting to authenticationContextClassReferences collection.</span></span>|


## <a name="properties"></a><span data-ttu-id="2f091-121">属性</span><span class="sxs-lookup"><span data-stu-id="2f091-121">Properties</span></span>

<span data-ttu-id="2f091-122">conditionalAccess 资源是条件访问对象模型的入口点，不包含任何属性。</span><span class="sxs-lookup"><span data-stu-id="2f091-122">The conditionalAccess resource is the entry point for the Conditional Access object model and doesn't contain any properties.</span></span>

## <a name="relationships"></a><span data-ttu-id="2f091-123">关系</span><span class="sxs-lookup"><span data-stu-id="2f091-123">Relationships</span></span>
| <span data-ttu-id="2f091-124">关系</span><span class="sxs-lookup"><span data-stu-id="2f091-124">Relationship</span></span> | <span data-ttu-id="2f091-125">类型</span><span class="sxs-lookup"><span data-stu-id="2f091-125">Type</span></span>   |<span data-ttu-id="2f091-126">说明</span><span class="sxs-lookup"><span data-stu-id="2f091-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f091-127">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2f091-127">conditionalAccessPolicy</span></span>|<span data-ttu-id="2f091-128">[conditionalAccessPolicy](conditionalaccesspolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f091-128">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span>| <span data-ttu-id="2f091-129">只读。</span><span class="sxs-lookup"><span data-stu-id="2f091-129">Read-only.</span></span> <span data-ttu-id="2f091-130">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2f091-130">Nullable.</span></span> <span data-ttu-id="2f091-131">返回指定的条件访问策略的集合。</span><span class="sxs-lookup"><span data-stu-id="2f091-131">Returns a collection of the specified Conditional Access policies.</span></span>|
|<span data-ttu-id="2f091-132">namedLocations</span><span class="sxs-lookup"><span data-stu-id="2f091-132">namedLocations</span></span>|<span data-ttu-id="2f091-133">[namedLocations](namedlocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f091-133">[namedLocations](namedlocation.md) collection</span></span>| <span data-ttu-id="2f091-134">只读。</span><span class="sxs-lookup"><span data-stu-id="2f091-134">Read-only.</span></span> <span data-ttu-id="2f091-135">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2f091-135">Nullable.</span></span> <span data-ttu-id="2f091-136">返回指定命名位置的集合。</span><span class="sxs-lookup"><span data-stu-id="2f091-136">Returns a collection of the specified named locations.</span></span>|
|<span data-ttu-id="2f091-137">authenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="2f091-137">authenticationContextClassReferences</span></span>|<span data-ttu-id="2f091-138">[authenticationContextClassReferences](authenticationcontextclassreference.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f091-138">[authenticationContextClassReferences](authenticationcontextclassreference.md) collection</span></span>|<span data-ttu-id="2f091-139">只读。</span><span class="sxs-lookup"><span data-stu-id="2f091-139">Read-only.</span></span> <span data-ttu-id="2f091-140">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2f091-140">Nullable.</span></span> <span data-ttu-id="2f091-141">返回指定的身份验证上下文类引用的集合。</span><span class="sxs-lookup"><span data-stu-id="2f091-141">Returns a collection of the specified authentication context class references.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditional access resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

