---
title: educationRoot 资源类型
description: '`/education` 命名空间公开特定于教育部门的功能。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 91f0162402b8c87042fab622710d314f27d6f4e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523510"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="37049-103">educationRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="37049-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37049-104">`/education` 命名空间公开特定于教育部门的功能。</span><span class="sxs-lookup"><span data-stu-id="37049-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="37049-105">`/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。</span><span class="sxs-lookup"><span data-stu-id="37049-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="37049-106">教育命名空间提供有关这些对象特定于教育的属性和功能。</span><span class="sxs-lookup"><span data-stu-id="37049-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="37049-107">方法</span><span class="sxs-lookup"><span data-stu-id="37049-107">Methods</span></span>

| <span data-ttu-id="37049-108">方法</span><span class="sxs-lookup"><span data-stu-id="37049-108">Method</span></span>           | <span data-ttu-id="37049-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="37049-109">Return Type</span></span>    |<span data-ttu-id="37049-110">说明</span><span class="sxs-lookup"><span data-stu-id="37049-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37049-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="37049-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="37049-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="37049-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="37049-113">通过发布到 classes 集合创建新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="37049-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="37049-114">List classes</span><span class="sxs-lookup"><span data-stu-id="37049-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="37049-115">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37049-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="37049-116">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="37049-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="37049-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="37049-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="37049-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="37049-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="37049-119">通过发布到 schools 集合创建新的 **educationSchool**。</span><span class="sxs-lookup"><span data-stu-id="37049-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="37049-120">List schools</span><span class="sxs-lookup"><span data-stu-id="37049-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="37049-121">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37049-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="37049-122">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="37049-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="37049-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="37049-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="37049-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="37049-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="37049-125">通过发布到 users 集合创建新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="37049-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="37049-126">List users</span><span class="sxs-lookup"><span data-stu-id="37049-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="37049-127">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37049-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="37049-128">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="37049-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="37049-129">属性</span><span class="sxs-lookup"><span data-stu-id="37049-129">Properties</span></span>
<span data-ttu-id="37049-130">无。</span><span class="sxs-lookup"><span data-stu-id="37049-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="37049-131">关系</span><span class="sxs-lookup"><span data-stu-id="37049-131">Relationships</span></span>
| <span data-ttu-id="37049-132">关系</span><span class="sxs-lookup"><span data-stu-id="37049-132">Relationship</span></span> | <span data-ttu-id="37049-133">类型</span><span class="sxs-lookup"><span data-stu-id="37049-133">Type</span></span>   |<span data-ttu-id="37049-134">说明</span><span class="sxs-lookup"><span data-stu-id="37049-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37049-135">classes</span><span class="sxs-lookup"><span data-stu-id="37049-135">classes</span></span>|<span data-ttu-id="37049-136">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37049-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="37049-p102">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="37049-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="37049-139">me</span><span class="sxs-lookup"><span data-stu-id="37049-139">me</span></span>|[<span data-ttu-id="37049-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="37049-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="37049-p103">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="37049-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="37049-143">schools</span><span class="sxs-lookup"><span data-stu-id="37049-143">schools</span></span>|<span data-ttu-id="37049-144">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37049-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="37049-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="37049-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="37049-147">users</span><span class="sxs-lookup"><span data-stu-id="37049-147">users</span></span>|<span data-ttu-id="37049-148">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37049-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="37049-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="37049-p105">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationroot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
