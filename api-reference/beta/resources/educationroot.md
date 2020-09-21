---
title: educationRoot 资源类型
description: '`/education` 命名空间公开特定于教育部门的功能。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a6f72f16d3a1e121883c4aa297aa0a4c93fe79d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989661"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="6842e-103">educationRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="6842e-103">educationRoot resource type</span></span>

<span data-ttu-id="6842e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6842e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6842e-105">`/education` 命名空间公开特定于教育部门的功能。</span><span class="sxs-lookup"><span data-stu-id="6842e-105">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="6842e-106">`/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。</span><span class="sxs-lookup"><span data-stu-id="6842e-106">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="6842e-107">教育命名空间提供有关这些对象特定于教育的属性和功能。</span><span class="sxs-lookup"><span data-stu-id="6842e-107">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="6842e-108">方法</span><span class="sxs-lookup"><span data-stu-id="6842e-108">Methods</span></span>

| <span data-ttu-id="6842e-109">方法</span><span class="sxs-lookup"><span data-stu-id="6842e-109">Method</span></span>           | <span data-ttu-id="6842e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6842e-110">Return Type</span></span>    |<span data-ttu-id="6842e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6842e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6842e-112">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="6842e-112">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="6842e-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="6842e-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="6842e-114">通过发布到 classes 集合创建新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="6842e-114">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="6842e-115">List classes</span><span class="sxs-lookup"><span data-stu-id="6842e-115">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="6842e-116">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6842e-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="6842e-117">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6842e-117">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="6842e-118">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="6842e-118">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="6842e-119">educationSchool</span><span class="sxs-lookup"><span data-stu-id="6842e-119">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="6842e-120">通过发布到 schools 集合创建新的 **educationSchool**。</span><span class="sxs-lookup"><span data-stu-id="6842e-120">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="6842e-121">List schools</span><span class="sxs-lookup"><span data-stu-id="6842e-121">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="6842e-122">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6842e-122">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="6842e-123">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6842e-123">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="6842e-124">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="6842e-124">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="6842e-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="6842e-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="6842e-126">通过发布到 users 集合创建新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="6842e-126">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="6842e-127">List users</span><span class="sxs-lookup"><span data-stu-id="6842e-127">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="6842e-128">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6842e-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="6842e-129">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6842e-129">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="6842e-130">属性</span><span class="sxs-lookup"><span data-stu-id="6842e-130">Properties</span></span>
<span data-ttu-id="6842e-131">无。</span><span class="sxs-lookup"><span data-stu-id="6842e-131">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="6842e-132">关系</span><span class="sxs-lookup"><span data-stu-id="6842e-132">Relationships</span></span>
| <span data-ttu-id="6842e-133">关系</span><span class="sxs-lookup"><span data-stu-id="6842e-133">Relationship</span></span> | <span data-ttu-id="6842e-134">类型</span><span class="sxs-lookup"><span data-stu-id="6842e-134">Type</span></span>   |<span data-ttu-id="6842e-135">说明</span><span class="sxs-lookup"><span data-stu-id="6842e-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6842e-136">classes</span><span class="sxs-lookup"><span data-stu-id="6842e-136">classes</span></span>|<span data-ttu-id="6842e-137">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6842e-137">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="6842e-p102">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="6842e-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="6842e-140">me</span><span class="sxs-lookup"><span data-stu-id="6842e-140">me</span></span>|[<span data-ttu-id="6842e-141">educationUser</span><span class="sxs-lookup"><span data-stu-id="6842e-141">educationUser</span></span>](educationuser.md)| <span data-ttu-id="6842e-p103">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="6842e-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="6842e-144">schools</span><span class="sxs-lookup"><span data-stu-id="6842e-144">schools</span></span>|<span data-ttu-id="6842e-145">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6842e-145">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="6842e-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="6842e-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="6842e-148">users</span><span class="sxs-lookup"><span data-stu-id="6842e-148">users</span></span>|<span data-ttu-id="6842e-149">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6842e-149">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="6842e-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="6842e-p105">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


