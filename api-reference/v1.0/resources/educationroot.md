---
title: educationRoot 资源类型
description: '`/education` 命名空间公开特定于教育部门的功能。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 69835ca7e3c7a45864382eab9d1b362034873a60
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277908"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="e43e6-103">educationRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="e43e6-103">educationRoot resource type</span></span>

<span data-ttu-id="e43e6-104">`/education` 命名空间公开特定于教育部门的功能。</span><span class="sxs-lookup"><span data-stu-id="e43e6-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="e43e6-105">`/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。</span><span class="sxs-lookup"><span data-stu-id="e43e6-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="e43e6-106">教育命名空间提供有关这些对象特定于教育的属性和功能。</span><span class="sxs-lookup"><span data-stu-id="e43e6-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="e43e6-107">方法</span><span class="sxs-lookup"><span data-stu-id="e43e6-107">Methods</span></span>

| <span data-ttu-id="e43e6-108">方法</span><span class="sxs-lookup"><span data-stu-id="e43e6-108">Method</span></span>           | <span data-ttu-id="e43e6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e43e6-109">Return Type</span></span>    |<span data-ttu-id="e43e6-110">说明</span><span class="sxs-lookup"><span data-stu-id="e43e6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e43e6-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="e43e6-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="e43e6-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="e43e6-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="e43e6-113">通过发布到 classes 集合创建新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="e43e6-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="e43e6-114">List classes</span><span class="sxs-lookup"><span data-stu-id="e43e6-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="e43e6-115">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e43e6-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="e43e6-116">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e43e6-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="e43e6-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="e43e6-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="e43e6-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="e43e6-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="e43e6-119">通过发布到 schools 集合创建新的 **educationSchool**。</span><span class="sxs-lookup"><span data-stu-id="e43e6-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="e43e6-120">List schools</span><span class="sxs-lookup"><span data-stu-id="e43e6-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="e43e6-121">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e43e6-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="e43e6-122">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e43e6-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="e43e6-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="e43e6-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="e43e6-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="e43e6-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e43e6-125">通过发布到 users 集合创建新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="e43e6-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="e43e6-126">List users</span><span class="sxs-lookup"><span data-stu-id="e43e6-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="e43e6-127">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e43e6-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="e43e6-128">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e43e6-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="e43e6-129">属性</span><span class="sxs-lookup"><span data-stu-id="e43e6-129">Properties</span></span>
<span data-ttu-id="e43e6-130">无。</span><span class="sxs-lookup"><span data-stu-id="e43e6-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="e43e6-131">关系</span><span class="sxs-lookup"><span data-stu-id="e43e6-131">Relationships</span></span>
| <span data-ttu-id="e43e6-132">关系</span><span class="sxs-lookup"><span data-stu-id="e43e6-132">Relationship</span></span> | <span data-ttu-id="e43e6-133">类型</span><span class="sxs-lookup"><span data-stu-id="e43e6-133">Type</span></span>   |<span data-ttu-id="e43e6-134">说明</span><span class="sxs-lookup"><span data-stu-id="e43e6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e43e6-135">classes</span><span class="sxs-lookup"><span data-stu-id="e43e6-135">classes</span></span>|<span data-ttu-id="e43e6-136">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e43e6-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="e43e6-137">只读。</span><span class="sxs-lookup"><span data-stu-id="e43e6-137">Read-only.</span></span> <span data-ttu-id="e43e6-138">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e43e6-138">Nullable.</span></span>|
|<span data-ttu-id="e43e6-139">me</span><span class="sxs-lookup"><span data-stu-id="e43e6-139">me</span></span>|[<span data-ttu-id="e43e6-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="e43e6-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e43e6-141">只读。</span><span class="sxs-lookup"><span data-stu-id="e43e6-141">Read-only.</span></span> <span data-ttu-id="e43e6-142">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e43e6-142">Nullable.</span></span>|
|<span data-ttu-id="e43e6-143">schools</span><span class="sxs-lookup"><span data-stu-id="e43e6-143">schools</span></span>|<span data-ttu-id="e43e6-144">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e43e6-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="e43e6-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e43e6-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="e43e6-147">users</span><span class="sxs-lookup"><span data-stu-id="e43e6-147">users</span></span>|<span data-ttu-id="e43e6-148">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e43e6-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="e43e6-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="e43e6-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e43e6-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e43e6-151">JSON representation</span></span>
<span data-ttu-id="e43e6-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e43e6-152">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```

<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e43e6-153">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e43e6-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e43e6-154">C#</span><span class="sxs-lookup"><span data-stu-id="e43e6-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_education-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e43e6-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="e43e6-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_education-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e43e6-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="e43e6-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_education-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/resources/educationroot.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/resources/educationroot.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/educationroot.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
